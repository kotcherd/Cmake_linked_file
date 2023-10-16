CMAKE_MINIMUM_REQUIRED(VERSION 3.2)

project(go Fortran)

add_executable(go main.F)

# get a list of files to compile #
# glob # file(GLOB go_src CONFIGURE_DEPENDS *.f90)

message(STATUS " " )
message(STATUS " " )
message(STATUS " " )
message(STATUS " " )

# glob # foreach(myFile ${go_src})
# glob #   message(STATUS "===> " ${myFile})
# glob # endforeach()

message(STATUS " " )
message(STATUS " " )
message(STATUS " " )
message(STATUS " " )

add_library(${PROJECT_NAME}-static STATIC )

target_sources(${PROJECT_NAME}-static PRIVATE five.f90 four.f90 one.f90 three.f90 two.f90 zero.f90)

target_link_libraries(go PUBLIC go-static)

