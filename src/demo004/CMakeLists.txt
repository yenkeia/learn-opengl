PROJECT(demo004)

FIND_PACKAGE(glfw3 REQUIRED)
FIND_PACKAGE(OpenGL REQUIRED)

SET(SOURCE_FILES main.cpp ../../lib/glad.c)

ADD_EXECUTABLE(demo004 ${SOURCE_FILES})

TARGET_LINK_LIBRARIES(demo004 glfw)
TARGET_LINK_LIBRARIES(demo004 OpenGL::GL)