cmake_minimum_required(VERSION 3.8)
project(RQ)

set(CMAKE_C_STANDARD 99)

set(INClUDE_DIR ./include)
set(LIB_DIR ./lib)

include_directories(${INClUDE_DIR})
link_directories(${LIB_DIR})

link_libraries(RaptorQ)

set(SOURCE_FILES main.c)
add_executable(RQ ${SOURCE_FILES})

target_link_libraries(RQ RaptorQ)
