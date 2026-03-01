cmake_minimum_required(VERSION 4.1)
project(MatrixTUI C)

set(CMAKE_C_STANDARD 11)

add_subdirectory(MatrixClientLibrary)

add_executable(MatrixTUI src/main.c)
target_link_libraries(MatrixTUI MatrixSDK)