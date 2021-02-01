cmake_minimum_required(VERSION 3.16)
project(lua)

set(CMAKE_C_STANDARD 99)

add_library(lua lapi.c lauxlib.c lbaselib.c lbitlib.c lcode.c lcorolib.c lctype.c ldblib.c ldebug.c ldo.c
        ldump.c lfunc.c lgc.c linit.c liolib.c llex.c lmathlib.c lmem.c loadlib.c lobject.c lopcodes.c
        loslib.c lparser.c lstate.c lstring.c lstrlib.c ltable.c ltablib.c ltests.c ltm.c lundump.c
        lutf8lib.c lvm.c lzio.c)

target_include_directories(lua PRIVATE .)