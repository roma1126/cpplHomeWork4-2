cmake_minimum_required(VERSION 3.20)
project(MyProject2)

add_subdirectory(../Catch2 Catch2-build)
add_executable(MyProjectTest2 test-main2.cpp)
target_link_libraries(MyProjectTest2 PRIVATE Catch2::Catch2)