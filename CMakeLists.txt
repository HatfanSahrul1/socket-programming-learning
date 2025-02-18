cmake_minimum_required(VERSION 3.10)
project(simple_socket)

set(CMAKE_CXX_STANDARD 14)

add_executable(server tcp/server_simple.cpp)
target_link_libraries(server pthread)

add_executable(client tcp/client_simple.cpp)
target_link_libraries(client pthread)

add_executable(udp_server udp/udp_server.cpp)
target_link_libraries(udp_server pthread)

add_executable(udp_client udp/udp_client.cpp)
target_link_libraries(udp_client pthread)