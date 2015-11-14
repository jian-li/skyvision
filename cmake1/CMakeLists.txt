cmake_minimum_required(VERSION 2.8)

find_package(OpenCV REQUIRED)

include_directories(OpenCV_INCLUDE_DIRS)

set(src ./DisplayImage.cpp)

add_executable(DisplayImage ${src})

target_link_libraries(DisplayImage ${OpenCV_LIBRARIES})

