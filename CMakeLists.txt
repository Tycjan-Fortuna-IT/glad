cmake_minimum_required(VERSION 3.16...3.26 FATAL_ERROR)

project(GLAD)

include_directories(${PROJECT_SOURCE_DIR}/include)

file(GLOB_RECURSE HEADERS "include/*.h")
file(GLOB_RECURSE SOURCES "src/*.c")

add_library(${PROJECT_NAME} STATIC ${HEADERS} ${SOURCES})
