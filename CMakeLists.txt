cmake_minimum_required(VERSION 2.8)
project(papaman)
FIND_LIBRARY(OPENGL_LIBRARY OpenGL)
FIND_LIBRARY(GLUT_LIBRARY GLUT)

set(sources 
		"src/main.cpp"
)

add_executable(papaman ${sources})
target_link_libraries(papaman ${OPENGL_LIBRARY} ${GLUT_LIBRARY})
#include_directories("./include/")
