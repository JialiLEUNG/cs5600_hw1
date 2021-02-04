cmake_minimum_required(VERSION 3.17)
project(assignment_1 C)

set(CMAKE_C_STANDARD 11)

# include and lib directories on MacOS
# adjust for Windows 10 or Linux
include_directories(/usr/local/include)
link_directories(/usr/local/lib)

add_executable(assignment_1 word.c alu.c assignment_1_test.c)
target_link_libraries(assignment_1 cunit)