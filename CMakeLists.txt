cmake_minimum_required(VERSION 2.8.12)
project(MagnumDemo)

add_definitions("-std=c++11")

include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
conan_basic_setup()

add_executable(demo demo.cpp)
target_link_libraries(demo ${CONAN_LIBS})

#install(TARGETS demo DESTINATION ${MAGNUM_BINARY_INSTALL_DIR})

