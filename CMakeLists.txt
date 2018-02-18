cmake_minimum_required(VERSION 3.8)
project(zmalloc)

set(CMAKE_CXX_STANDARD 11)

file(GLOB SOURCES
        *.h
        *.cpp
        )

add_library(zmalloc ${SOURCES})


install(TARGETS zmalloc
        RUNTIME DESTINATION bin
        LIBRARY DESTINATION lib
        ARCHIVE DESTINATION libstatic)

install(FILES ${PROJECT_SOURCE_DIR}/zmalloc.h DESTINATION include)
