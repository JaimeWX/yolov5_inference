cmake_minimum_required(VERSION 3.10)

project(yolov5_cv)

set(OpenCV_DIR /home/jaime/opencv-4.5.5/build)
find_package(OpenCV REQUIRED)
INCLUDE_DIRECTORIES(${OpenCV_INCLUDE_DIRS})

add_executable(yolov5_cv yolov5_cv.cpp)

target_link_libraries(yolov5_cv ${OpenCV_LIBS} )