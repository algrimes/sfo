cmake_minimum_required(VERSION 3.20)

project(sfo
    DESCRIPTION "PARAM.SFO Manager for PS4"
    HOMEPAGE_URL https://github.com/hippe68/sfo
    VERSION 1.03
    LANGUAGES C
)

add_executable(${PROJECT_NAME} sfo.c)

set_target_properties(${PROJECT_NAME}
    PROPERTIES
    C_STANDARD 17
    RUNTIME_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/bin"
)

install(TARGETS sfo RUNTIME DESTINATION bin)