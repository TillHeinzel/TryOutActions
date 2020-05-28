cmake_minimum_required(VERSION 3.16)
project(TryOutActions)

add_executable(TryOutActions main.cpp)

install(TARGETS main)

enable_testing()
add_test(NAME main COMMAND main)