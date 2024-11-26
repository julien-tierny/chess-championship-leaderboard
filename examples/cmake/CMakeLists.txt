cmake_minimum_required(VERSION 3.15...3.31)

project(myCoolProject
  VERSION 1.0
  LANGUAGES CXX)

include_directories(.)

add_library(myLibExample Foo.cpp Foo.h)

add_executable(myCoolProgram main.cpp)

target_link_libraries(myCoolProgram PRIVATE myLibExample)
