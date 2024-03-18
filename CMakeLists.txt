cmake_minimum_required(VERSION 3.24)
project(zynth53
    VERSION 0.1.0
    DESCRIPTION "Si5351 Library"
    LANGUAGES C CXX
)
set(CMAKE_C_STANDARD 17)
set(CMAKE_CXX_STANDARD 20)
cmake_policy(SET CMP0135 NEW)

include_directories(include)
add_subdirectory(src)
add_subdirectory(tests)
