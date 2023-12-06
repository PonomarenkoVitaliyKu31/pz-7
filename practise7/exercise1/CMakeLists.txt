cmake_minimum_required(VERSION 3.26)
project(exercise1 C)

set(CMAKE_C_STANDARD 11)

add_executable(exercise1 program_parent.c
        program_child.c)
