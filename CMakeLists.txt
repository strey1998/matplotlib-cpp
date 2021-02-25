cmake_minimum_required (VERSION 3.15)

find_package(Python3 COMPONENTS Development)

add_library(matplotlib-cpp INTERFACE)
set_target_properties(matplotlib-cpp PROPERTIES LINKER_LANGUAGE CXX)
target_link_libraries(matplotlib-cpp PUBLIC Python3::Python)
target_include_directories(matplotlib-cpp PUBLIC .)
