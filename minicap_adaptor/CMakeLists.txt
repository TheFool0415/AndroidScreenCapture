cmake_minimum_required(VERSION 3.7)
project(minicap_adaptor)

#set(CMAKE_CXX_STANDARD 11)
#set(CMAKE_CXX_FLAGS ${CMAKE_CXX_FLAGS} "-std=c++1y -pthread -O2")
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++1y -pthread")
#set(CMAKE_LINK_LIBRARY_FLAG ${CMAKE_LINK_LIBRARY_FLAG} "-pthread")

set(SOURCE_FILES main.cpp unsock.cpp)
add_executable(minicap_adaptor ${SOURCE_FILES})
#message(ENABLED_LANGUAGES)
message(COMPILER " " ${CMAKE_CXX_COMPILER})
message(ABI " " ${CMAKE_CXX_COMPILER_ABI})
message(ID " " ${CMAKE_CXX_COMPILER_ID})
#message(${CMAKE_CXX_COMPILER_LAUNCHER})
#message(${CMAKE_CXX_COMPILER_EXTERNAL_TOOLCHAIN})
message(LOADED " " ${CMAKE_CXX_COMPILER_LOADED})
message(VERSION " " ${CMAKE_CXX_COMPILER_VERSION})
#message(${CMAKE_CXX_COMPILER_TARGET})
message(CROSS " " ${CMAKE_CROSSCOMPILING})
