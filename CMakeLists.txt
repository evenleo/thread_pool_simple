cmake_minimum_required(VERSION 3.11)
project(even)

SET(CMAKE_BUILD_TYPE "Debug")
SET(CMAKE_CXX_FLAGS_DEBUG "$ENV{CXXFLAGS} -O0 -Wall -g2 -ggdb")
SET(CMAKE_CXX_FLAGS_RELEASE "$ENV{CXXFLAGS} -O3 -Wall")

set(SOURCE_FILES  thread_pool_simple.c)
add_executable(even ${SOURCE_FILES} )

TARGET_LINK_LIBRARIES(even pthread)
