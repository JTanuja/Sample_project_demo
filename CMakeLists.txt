cmake_minimum_required(VERSION 3.22) 

project("Hello") 

include_directories(lib) 
add_library(calc lib/calculate.cpp) 
add_executable(main main.cpp) 
target_link_libraries(main calc)


