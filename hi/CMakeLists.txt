cmake_minimum_required(VERSION 3.8)
project(hi)
add_executable(hi hi.cpp)
target_link_directories(hi 
PRIVATE ${CMAKE_SOURCE_DIR}/lib
PRIVATE ${CMAKE_SOURCE_DIR}/include
)
target_link_libraries(hi PRIVATE bob)

