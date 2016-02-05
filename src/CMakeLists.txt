set(SOURCE_FILES main.cpp)
add_executable(white ${SOURCE_FILES})

target_link_libraries(white ${OPENGL_LIBRARIES})
add_definitions(-DGLEW_STATIC)
target_link_libraries(white libglew_shared)
target_link_libraries(white ${GLFW_LIBRARIES} glfw)