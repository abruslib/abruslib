cmake_minimum_required(VERSION 3.10)

project(example)

add_subdirectory(
    3rd_party/abruslib
)

add_executable(example
    src/example.c
)

target_link_libraries(example PUBLIC abruslib)

