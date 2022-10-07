cmake_minimum_required(VERSION 3.0)

PROJECT(sofa VERSION 15.0)

FILE(GLOB SOFA_SRC src/*.c)
FILE(GLOB SOFA_HEADERS src/*.h)


add_library(sofa STATIC ${SOFA_SRC})

target_include_directories(sofa PUBLIC src)

install(TARGETS sofa DESTINATION ${CMAKE_INSTALL_PREFIX}/lib)
install(FILES ${SOFA_HEADERS} DESTINATION ${CMAKE_INSTALL_PREFIX}/include)
