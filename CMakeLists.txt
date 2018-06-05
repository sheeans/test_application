cmake_minimum_required(VERSION 2.8)


set(TARGET audio-router)
project(${TARGET})


set(DIR ${CMAKE_CURRENT_SOURCE_DIR})


set(SRCS ${DIR}/audio_router.c)

add_executable(${TARGET} ${SRCS})

target_link_libraries(${TARGET} asound)
target_link_libraries(${TARGET} dlt)
