cmake_minimum_required(VERSION 3.10 FATAL_ERROR)
project(lua VERSION 5.1.1)
add_library(
    lua
    lapi.c
    lapi.h
    lauxlib.c
    lauxlib.h
    lbaselib.c
    lcode.c
    lcode.h
    ldblib.c
    ldebug.c
    ldebug.h
    ldo.c
    ldo.h
    ldump.c
    lfunc.c
    lfunc.h
    lgc.c
    lgc.h
    linit.c
    liolib.c
    llex.c
    llex.h
    llimits.h
    lmathlib.c
    lmem.c
    lmem.h
    loadlib.c
    lobject.c
    lobject.h
    lopcodes.c
    lopcodes.h
    loslib.c
    lparser.c
    lparser.h
    lstate.c
    lstate.h
    lstring.c
    lstring.h
    lstrlib.c
    ltable.c
    ltable.h
    ltablib.c
    ltests.c
    ltests.h
    ltm.c
    ltm.h
    luaconf.h
    lualib.h
    lundump.c
    lundump.h
    lvm.c
    lvm.h
    lzio.c
    lzio.h
)

file(COPY ${CMAKE_CURRENT_SOURCE_DIR}
     DESTINATION "${CMAKE_CURRENT_BINARY_DIR}/include"
     FILES_MATCHING PATTERN "*.h")
