add_library(Environment INTERFACE)

target_include_directories(Environment INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/include)

add_subdirectory(tests)