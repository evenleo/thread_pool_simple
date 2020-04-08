cmake_minimum_required(VERSION 3.11)
project(thread_pool_example)

add_executable(thread_pool_example thread_pool_example.cpp)

TARGET_LINK_LIBRARIES(thread_pool_example -lpthread)

