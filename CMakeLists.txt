cmake_minimum_required(VERSION 3.12)
project(MyPaint)

set(CMAKE_CXX_STANDARD 11)

set(CMAKE_VERBOSE_MAKEFILE TRUE)
set(EXECUTABLE_OUTPUT_PATH ${CMAKE_CURRENT_SOURCE_DIR})

set(NAME MyPaint)

set(SRCS srcs/main.cpp)

add_executable(${NAME} WIN32 ${SRCS})
target_link_libraries(${NAME} -municode)
