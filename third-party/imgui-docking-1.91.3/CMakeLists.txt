cmake_minimum_required(VERSION 3.15)

project(imnodes)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

add_library(imgui)
target_sources(imgui PRIVATE
    imgui.cpp 
    imgui_demo.cpp 
    imgui_draw.cpp 
    imgui_tables.cpp 
    imgui_widgets.cpp 
    backends/imgui_impl_sdl3.cpp 
    backends/imgui_impl_vulkan.cpp
)
target_include_directories(imgui PUBLIC ${CMAKE_CURRENT_SOURCE_DIR} ${CMAKE_CURRENT_SOURCE_DIR}/backends)