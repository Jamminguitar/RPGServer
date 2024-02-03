cmake_minimum_required(VERSION 3.14)


project(
    rpg_server
    VERSION 0.1
    LANGUAGES CXX)

set(sources ${sources} 
    src/main.cpp
)

ADD_SUBDIRECTORY(libs)
add_executable(rpg_server ${sources})
TARGET_LINK_LIBRARIES(
   rpg_server PRIVATE
   asio
)
