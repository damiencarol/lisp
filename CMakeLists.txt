cmake_minimum_required(VERSION 3.9)

project(lisp)

add_library(mpc STATIC src/mpc.c)
add_executable(${PROJECT_NAME} src/main.c)
target_link_libraries(${PROJECT_NAME} readline)
target_link_libraries(${PROJECT_NAME} mpc)


add_test(TestName ${PROJECT_NAME})
add_custom_target(check COMMAND ${CMAKE_CTEST_COMMAND}
                  DEPENDS ${PROJECT_NAME})