project(chatCommon)

add_executable(${PROJECT_NAME} common.cpp)
target_link_libraries(${PROJECT_NAME} SQLiteCpp sqlite3 fmt pthread)
