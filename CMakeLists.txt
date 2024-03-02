cmake_minimum_required(VERSION 3.28.3)

project(GLFW_Demo VERSION 1.0.0)

add_subdirectory(glfw)

add_executable(MyApp main.cpp)

target_link_libraries(MyApp glfw)

find_package(OpenGL REQUIRED)

target_link_libraries(MyApp OpenGL::GL)