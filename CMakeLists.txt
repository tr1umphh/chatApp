cmake_minimum_required(VERSION 3.27)
project(chat VERSION 1.0)

set(CMAKE_CXX_STANDARD 20)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
link_directories(${Boost_LIBRARY_DIRS})

find_package(Boost 1.65.1 REQUIRED)

enable_testing()
add_subdirectory(thirdparty/SQLiteCpp)
add_subdirectory(thirdparty/GameNetworkingSockets)
add_subdirectory(thirdparty/fmt)
add_subdirectory(chatCommon)
add_subdirectory(chatClient)

add_compile_options(-g -Wall)
