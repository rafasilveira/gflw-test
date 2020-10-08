cmake_minimum_required(VERSION 3.10.2)
set(CMAKE_CXX_STANDARD 17)
project(GLFW-Test)

include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
conan_basic_setup()

add_executable(glfw-test src/main.cpp)

target_link_libraries(glfw-test ${CONAN_LIBS})
