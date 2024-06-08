cmake_minimum_required( VERSION 3.20 )

project( yocto_test_app
        VERSION 1.0.0
        LANGUAGES C
)

add_executable( yocto_test_app main.c )

target_compile_options( yocto_test_app PRIVATE
        -Wall
        -Wextra
        -Wpedantic
        -Ofast
)
