# C++ Project Template

Template for a CMake C++20 project with Google style format and
not overly restrictive clang-tidy configuration.

## Build

```console
$ make -B build -DCMAKE_BUILD_TYPE=Release -DCMAKE_EXPORT_COMPILE_COMMANDS=On -G Ninja
-- Configuring done
-- Generating done
-- Build files have been written to: proj_template/build
$ cmake --build build
[2/2] Linking CXX executable main
$ build/main
Hello, World!
```

Clang Tidy:

```console
$ cd build
$ clang-tidy ../main.cpp
44851 warnings generated.
Suppressed 44851 warnings (44851 in non-user code).
Use -header-filter=.* to display errors from all non-system headers. Use -system-headers to display errors from system headers as well.
```

Clang Format (dry-run):

```console
$ clang-format -n main.cpp
$
```
