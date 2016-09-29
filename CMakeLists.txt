cmake_minimum_required(VERSION 3.3)

project(boost_fusion)

add_library(boost_fusion INTERFACE)

target_include_directories(boost_fusion BEFORE INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/include)

install(TARGETS boost_fusion DESTINATION lib)
install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/include/boost DESTINATION include)
