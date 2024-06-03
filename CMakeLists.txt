cmake_minimum_required(VERSION 3.10)
project(game_project)

set(CMAKE_TOOLCHAIN_FILE "C:/vcpkg/scripts/buildsystems/vcpkg.cmake")

add_executable(game_project src/main.cpp)

find_package(SFML 2.5 COMPONENTS system window graphics network audio REQUIRED)
target_link_libraries(game_project sfml-system sfml-window sfml-graphics sfml-network sfml-audio)