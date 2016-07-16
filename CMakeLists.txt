#cmake_minimum_required(VERSION 3.5)

project(GeneralPool)

add_library( ${PROJECT_NAME} STATIC Pool.cpp)

add_executable( ${PROJECT_NAME}_main main.cpp)

MESSAGE( STATUS "CMAKE_BINARY_DIR:         " ${PROJECT_NAME} )

target_link_libraries( ${PROJECT_NAME}_main ${PROJECT_NAME} )


