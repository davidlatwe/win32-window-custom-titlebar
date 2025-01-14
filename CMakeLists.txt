cmake_minimum_required(VERSION 3.20)
project(win32_window_custom_titlebar C)

set(CMAKE_C_STANDARD 11)

add_executable(main
    WIN32
    main.c)


target_compile_options(main
    PRIVATE
    /nologo /Od /Zo /Zi /FC /std:c11
    /Wall /wd4100 /wd4255 /wd5105 /wd5045 /wd4819 /wd4710 /WX
    /D UNICODE
    /D _UNICODE
)
