cmake_minimum_required (VERSION 2.8)

project(test-external-project)

message("INSTALL_PRFIX is ${CMAKE_INSTALL_PREFIX}")

if ( SETUP_INSTALL )
    install (FILES 
            example.txt
        COMPONENT Runtime
        DESTINATION test-external-project
    )
endif()