cmake_minimum_required(VERSION 2.8)
project(galaxy)

add_subdirectory(bodies/saturn)
add_subdirectory(bodies/jupiter)
add_subdirectory(bodies/pluto)

add_custom_target(galaxy REQUIRED DEPENDS saturn jupiter pluto)
