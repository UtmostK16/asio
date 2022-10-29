cmake_minimum_required(VERSION 3.5)

project(JCASIO)

set(PRODUCT_BIN_DIR ${CMAKE_CURRENT_SOURCE_DIR}/product/bin)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(ASIO_INCLUDE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/asio-1.24.0/include)


add_subdirectory(tutorial)
