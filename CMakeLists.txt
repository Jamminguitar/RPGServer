cmake_minimum_required(VERSION 3.14)


project(
    rpg_server
    VERSION 0.1
    LANGUAGES CXX)

set(sources ${sources} 
    src/main.cpp
    libs/asio-1.28.0/include/asio.hpp
)

add_executable(rpg_server ${sources})