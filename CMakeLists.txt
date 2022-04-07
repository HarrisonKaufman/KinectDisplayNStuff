cmake_minimum_required(VERSION 3.21)
project(KinectDisplayNStuff)

set(CMAKE_CXX_STANDARD 14)

set("OpenCV_DIR" "C:/Users/omaha/CLionProjects/KinectDisplayNStuff/opencv/build/x64/vc15/lib")

find_package(OpenCV REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(KinectDisplayNStuff main.cpp)
target_link_libraries(KinectDisplayNStuff ${OpenCV_LIBS})