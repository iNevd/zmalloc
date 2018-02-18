cmake_minimum_required(VERSION 3.8)
project(zmalloc)

set(CMAKE_CXX_STANDARD 11)

file(GLOB SOURCES_FIRE_CORE
        *.h
        *.cpp
        )

add_library(zmalloc ${SOURCES_FIRE_CORE})