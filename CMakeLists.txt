cmake_minimum_required(VERSION 3.16)
project(TryOutActions)

set(CMAKE_PREFIX_PATH "dependencies")

find_package(Boost 1.73 REQUIRED MODULES headers coroutine context)

add_executable(TryOutActions main.cpp)

install(TARGETS TryOutActions)

enable_testing()
add_test(NAME main COMMAND main)