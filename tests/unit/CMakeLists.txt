cmake_minimum_required(VERSION 3.10)

project(unittests)

add_subdirectory(3rd_party/abruslib)
add_subdirectory(3rd_party/googletest)

add_executable(unittests
    src/tests.cpp
)

target_link_libraries(unittests PUBLIC abruslib gtest)