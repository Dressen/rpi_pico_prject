cmake_minimum_required(VERSION 3.22)

include(pico_sdk_import.cmake)

project(pico_projects)

pico_sdk_init()

add_executable(pico_starter
pico_starter.c
)

target_link_libraries(pico_starter pico_stdlib)

pico_add_extra_outputs(pico_starter)