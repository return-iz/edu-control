cmake_minimum_required(VERSION 3.2)

project(Edu-Control)

add_executable(
	EduControl
	main.cpp
)

target_link_libraries(EduControl glfw)

target_link_libraries(EduControl glad)

set(GLFW_BUILD_DOCS OFF CACHE BOOL "" FORCE)
set(GLFW_BUILD_TESTS OFF CACHE BOOL "" FORCE)
set(GLFW_BUILD_EXAMPLES OFF CACHE BOOL "" FORCE)

add_subdirectory(glfw-3.3.2)

add_subdirectory(glad)