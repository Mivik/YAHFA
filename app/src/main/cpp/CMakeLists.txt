
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fno-exceptions -fno-rtti")

cmake_minimum_required(VERSION 3.4.1)

aux_source_directory(src SRC_LIST)
add_library(yahfa SHARED ${SRC_LIST})

target_link_libraries(yahfa android log)
