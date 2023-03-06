cmake_minimum_required(VERSION 3.16)
project(fmt-test LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

find_package(fmt REQUIRED)

add_executable(fmt-test main.cpp)
target_link_libraries(fmt-test PRIVATE fmt::fmt)
