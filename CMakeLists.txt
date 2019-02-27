cmake_minimum_required(VERSION 3.9)

add_library(mpc STATIC src/mpc.c)
add_executable(lisp src/main.c)
target_link_libraries(lisp readline)
target_link_libraries(lisp mpc)


add_test(TestName lisp)
add_custom_target(check COMMAND ${CMAKE_CTEST_COMMAND}
                  DEPENDS lisp)