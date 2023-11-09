cmake_minimum_required(VERSION 3.16)
project(automata_exercise
  VERSION 0.0.1
  LANGUAGES CXX
)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)

add_subdirectory(source)

find_package(Catch2 3 REQUIRED) # add 'PATHS /path/to/local/install' if required.  
add_subdirectory(test)
