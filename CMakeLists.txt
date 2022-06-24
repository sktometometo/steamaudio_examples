cmake_minimum_required(VERSION 2.8)
project(steamaudio_examples)

set(STEAMAUDIO_DIRECTORY "${CMAKE_CURRENT_SOURCE_DIR}/steamaudio")

include_directories("${STEAMAUDIO_DIRECTORY}/include")
link_directories("${STEAMAUDIO_DIRECTORY}/lib/linux-x64")

add_executable(sample_01 examples/sample_01.cpp)
target_link_libraries(sample_01 phonon)
