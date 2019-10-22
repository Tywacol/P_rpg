cmake_minimum_required(VERSION 3.13)
project(P_rpg)

set(CMAKE_CXX_STANDARD 14)

set(SFML_DIR "/usr/lib/cmake/SFML")

find_package(SFML 2.5 COMPONENTS graphics audio REQUIRED)
add_executable(P_rpg main.cpp AI.cpp AI.hpp)
target_link_libraries(P_rpg sfml-graphics sfml-audio)