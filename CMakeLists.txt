cmake_minimum_required(VERSION 2.8)
project( DisplayImage )

add_executable( DisplayImage DisplayImage.cpp )

find_package(OpenCV REQUIRED PATHS ${PROJECT_SOURCE_DIR}/opencv_install)
include_directories( ${OpenCV_INCLUDE_DIRS} )

target_link_libraries( DisplayImage ${OpenCV_LIBS} )
target_compile_options(DisplayImage PUBLIC -std=c++11)

