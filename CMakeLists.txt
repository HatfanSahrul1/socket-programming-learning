cmake_minimum_required(VERSION 3.10)
project(simple_socket)

set(CMAKE_CXX_STANDARD 14)

add_executable(server src/server_simple.cpp)
target_link_libraries(server pthread)

add_executable(client src/client_simple.cpp)
target_link_libraries(client pthread)

