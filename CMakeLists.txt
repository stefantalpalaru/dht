# CMake-4 got even crazier and errors out if the minimum required version is
# lower than 3.5. Yes, you read that right - they redefined boolean logic :-)
cmake_minimum_required(VERSION 3.5)
project(dht C)

add_library(${PROJECT_NAME} STATIC
    dht.c
)

install(TARGETS ${PROJECT_NAME} DESTINATION lib)
install(FILES dht.h DESTINATION include/dht)
