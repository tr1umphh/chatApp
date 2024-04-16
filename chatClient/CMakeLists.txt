project(
  ChatAppClient
  VERSION 1.0.0
  LANGUAGES CXX)

set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

find_package(
  Qt5
  COMPONENTS Widgets
  REQUIRED)

add_executable(${PROJECT_NAME} mainwindow.cpp client.cpp mainwindow.h)

target_link_libraries(${PROJECT_NAME} Qt5::Widgets)
