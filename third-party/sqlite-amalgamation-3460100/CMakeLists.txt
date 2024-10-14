cmake_minimum_required(VERSION 3.15)

project(sqlite C)

set(CMAKE_C_STANDARD 99)

add_library(sqlite3)
target_sources(sqlite3 PRIVATE 
    sqlite3.c
)
target_include_directories(sqlite3 PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})