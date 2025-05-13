cmake_minimum_required(3.30.5)

project("Hello")

include_directories(lib)
add_library(calc lib/calculate.cpp)

add_executable(a.out main.cpp)
target_link_libraries(a.out calc)

