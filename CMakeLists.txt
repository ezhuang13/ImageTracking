cmake_minimum_required(VERSION 2.8)

project( DisplayImage )
SET(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -std=c++17 -g ")
find_package( OpenCV REQUIRED )

add_executable( SampleTracking SampleTracking.cpp )



target_link_libraries( SampleTracking ${OpenCV_LIBS} )
