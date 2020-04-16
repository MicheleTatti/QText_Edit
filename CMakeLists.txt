cmake_minimum_required(VERSION 3.15)
project(QText_Edit)

set(CMAKE_CXX_STANDARD 14)

include_directories(.)

set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

find_package(Qt5Core REQUIRED)
find_package(Qt5Widgets REQUIRED)
find_package(Qt5Gui REQUIRED)

set(SOURCE_FILE main.cpp textedit.cpp textedit.qrc)

add_executable(QText_Edit
        textedit.ui
        main.cpp
        textedit.h
        textedit.cpp
        textedit.qrc
        )

target_link_libraries(QText_Edit Qt5::Core Qt5::Widgets Qt5::Gui)



