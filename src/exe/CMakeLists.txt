project(${project_name}-exe C CXX)

add_executable(${project_name}-c-exe test.c)

target_link_libraries(${project_name}-c-exe
    PRIVATE ${project_name}-lib)

add_executable(${project_name}-cpp-exe test.cpp)

target_link_libraries(${project_name}-cpp-exe
    PRIVATE ${project_name}-lib)