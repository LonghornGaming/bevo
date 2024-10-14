set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED True)

add_executable(bevo)

target_sources(bevo PRIVATE 
    main.cpp
)
target_link_libraries(bevo PRIVATE fmt::fmt flecs::flecs_static sqlite3 SDL3::SDL3-static imgui imnodes)