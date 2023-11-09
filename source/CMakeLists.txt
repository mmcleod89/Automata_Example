add_library(Automata_lib automaton.cpp)
target_include_directories(Automata_lib PUBLIC ${CMAKE_SOURCE_DIR}/include)

add_executable(automata_examples main.cpp)
target_link_libraries(automata_examples Automata_lib)