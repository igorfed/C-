cmake_minimum_required (VERSION 2.8)

project(hello)

find_packages (OpenCV REQUIRED)

include_directories (${OpenCV_INCLUDE_DIRS})

add_executable(cv_hello hello.cpp)

target_link_libraries (cv_hello, ${OpenCV_LIBS})