cmake_minimum_required(VERSION 3.15)
PROJECT(hello)
ADD_SUBDIRECTORY(src bin)

INSTALL(FILES COPYRIGHT README.md DESTINATION share/doc/cmake/hello)
INSTALL(PROGRAMS runhello.sh DESTINATION bin)
INSTALL(DIRECTORY doc/ DESTINATION share/doc/cmake/hello)
