cmake_minimum_required(VERSION 3.5)

set(srcs "library/BitBuffer.cpp"
         "library/QrCode.cpp"
         "library/QrSegment.cpp"
         )


#set(SUPPORTED_TARGETS esp32)
#include($ENV{IDF_PATH}/tools/cmake/project.cmake)

idf_component_register(SRCS ${srcs}
                    INCLUDE_DIRS include
                    )


#register_component()
