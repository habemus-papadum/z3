################################################################################
# Example C++ project
################################################################################
project(Z3_CXX_INLINE_EXAMPLE CXX)
set(CMAKE_VERBOSE_MAKEFILE ON)
cmake_minimum_required(VERSION 2.8.12)

add_executable(cpp_example_inline example.cpp)
target_include_directories(cpp_example_inline PUBLIC ${CMAKE_SOURCE_DIR}/src/api
        ${CMAKE_SOURCE_DIR}/src/api/c++)
target_link_libraries(cpp_example_inline libz3)

