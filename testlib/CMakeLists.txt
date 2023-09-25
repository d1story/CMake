cmake_minimum_required(VERSION 3.6)
project(bob)
add_library(bob adder.cpp)
set_target_properties(bob PROPERTIES PUBLIC_HEADER adder.h)
install(TARGETS bob DESTINATION ${CMAKE_SOURCE_DIR}/lib
    PUBLIC_HEADER DESTINATION ${CMAKE_SOURCE_DIR}/include
)