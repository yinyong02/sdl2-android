cmake_minimum_required(VERSION 3.6)

project(MY_APP)

#shared library
#find_library(SDL2 SDL2)
#add_library(main SHARED)

#static library
find_library(SDL2 SDL2_main)
add_library(main STATIC)

target_sources(main PRIVATE main.c)

#link static library


target_link_libraries(main SDL2)


