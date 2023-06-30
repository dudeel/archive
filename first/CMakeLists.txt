cmake_minimum_required(VERSION 3.5)

project(untitled)

set(CMAKE_PREFIX_PATH "$ENV{QTDIR}")
find_package(Qt5Core REQUIRED)
find_package(Qt5Widgets REQUIRED)

set(CMAKE_INCLUDE_CURRENT_DIR "YES")
set(CMAKE_AUTOMOC "YES")
set(CMAKE_AUTOUIC "YES")

add_executable(${PROJECT_NAME} main.cpp
    form.h
    form.cpp
    form.ui
    )

target_link_libraries(${PROJECT_NAME} Qt5::Core Qt5::Widgets)
