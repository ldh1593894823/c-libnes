add_library(nes "")

target_sources(nes
    PRIVATE
        ${CMAKE_CURRENT_LIST_DIR}/bus.c
        ${CMAKE_CURRENT_LIST_DIR}/cpu.c
        ${CMAKE_CURRENT_LIST_DIR}/rom.c
    PUBLIC
        ${CMAKE_CURRENT_LIST_DIR}/bus.h
        ${CMAKE_CURRENT_LIST_DIR}/cpu.h
        ${CMAKE_CURRENT_LIST_DIR}/rom.h
        ${CMAKE_CURRENT_LIST_DIR}/nes.h
)

target_include_directories(nes
    PUBLIC
        ${CMAKE_CURRENT_LIST_DIR}
)