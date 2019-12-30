cmake_minimum_required(VERSION 3.15)
project(Tests)

enable_testing()

find_package(Boost REQUIRED)

add_subdirectory(src build/src)
add_subdirectory(test build/test)