cmake_minimum_required (VERSION 3.15)

add_library(matplotlib-cpp matplotlibcpp.h)
set_target_properties(matplotlib-cpp PROPERTIES LINKER_LANGUAGE CXX)
target_include_directories(matplotlib-cpp PUBLIC .)
