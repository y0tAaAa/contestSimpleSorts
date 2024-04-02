cmake_minimum_required(VERSION 3.27)
project(SimpleSorts C)
set(ERROR_FLAGS "-Werror -Wall")
set(CUSTOM_ERROR_FLAGS "-Werror=vla")
set(OPTIMIZATION_FLAGS "-march=native")

set(CMAKE_C_STANDARD 23)
set(CMAKE_C_STANDARD_REQUIRED ON)
set(CMAKE_C_FLAGS ${ERROR_FLAGS}\ ${CUSTOM_ERROR_FLAGS}\ ${OPTIMIZATION_FLAGS})
add_executable(SimpleSorts main.c
        insertion.c)
