cmake_minimum_required(VERSION 3.19 FATAL_ERROR)

set(PROJECT_NAME freeglut)
project(${PROJECT_NAME})

#set(CMALE_CXX_STANDART-17)

add_executable(${PROJECT_NAME} src/main.cpp)

add_subdirectory(GL)
target_link_libraries(${PROJECT_NAME} freeglut)

