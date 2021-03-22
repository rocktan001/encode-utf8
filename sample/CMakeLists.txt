cmake_minimum_required(VERSION 3.17) 
 
project(simplest)  

set(CMAKE_CXX_STANDARD 11) 

add_executable(simplest simplest_mediadata_main.cpp simplest_mediadata_h264.cpp simplest_mediadata_raw.cpp simplest_mediadata_aac.cpp simplest_mediadata_flv.cpp simplest_mediadata_udp.cpp)

# 添加链接库
TARGET_LINK_LIBRARIES(simplest ws2_32)
