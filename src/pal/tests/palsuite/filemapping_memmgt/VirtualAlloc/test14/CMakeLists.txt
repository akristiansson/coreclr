cmake_minimum_required(VERSION 2.8.12.2)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(SOURCES
  VirtualAlloc.cpp
)

add_executable(paltest_virtualalloc_test14
  ${SOURCES}
)

add_dependencies(paltest_virtualalloc_test14 coreclrpal)

target_link_libraries(paltest_virtualalloc_test14
  ${COMMON_TEST_LIBRARIES}
)
