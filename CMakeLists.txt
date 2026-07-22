cmake_minimum_required(VERSION 3.15)
project(PreyPredatorModel)

set(CMAKE_CXX_STANDARD 23)
set(CMAKE_CXX_STANDARD_REQUIRED True)

enable_testing() 

add_subdirectory(gtest)
add_subdirectory(src)

add_executable(Main src/main.cpp)

target_link_libraries(Main PRIVATE Environment)