cmake_minimum_required(VERSION 3.26)
project(exercise2 C)

set(CMAKE_C_STANDARD 11)

add_executable(exercise2 program_parent.c
        program_child.c)
