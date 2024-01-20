cmake_minimum_required(VERSION 3.21)
project(playground LANGUAGES CXX)

add_executable(main main.cpp)
set_property(TARGET main PROPERTY CXX_STANDARD 20)
