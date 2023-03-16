cmake_minimum_required(VERSION "3.17")

project(OpenCVCplusCplus)

set(OpenCV_DIR /usr/local/Cellar/opencv/4.7.0_2)

set(CMAKE_CXX_STANDARD 14)

find_package(OpenCV REQUIRED)

include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(OpenCVCplusCplus main.cpp)

target_link_libraries(OpenCVCplusCplus ${OpenCV_LIBS})