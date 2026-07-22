add_executable(EnvironmentTests 
    Environment_test.cpp 
    EnvironmentFabric_tests.cpp
)

target_link_libraries(EnvironmentTests PRIVATE Environment gtest_main)

add_test(NAME EnvironmentTests COMMAND EnvironmentTests)