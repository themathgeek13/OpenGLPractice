file(GLOB Sources "*.cpp")

# Sources #
set(MY_HEADER_FILES
        ${MY_HEADER_FILES}
        GraphicsManager.hpp
        Color.hpp
        Mesh.hpp
        )

set(MY_SOURCE_FILES
        ${MY_SOURCE_FILES}
        main.cpp
        GraphicsManager.cpp
        Mesh.cpp
        )

add_executable(OpenGLPractice
        ${MY_HEADER_FILES}
        ${MY_SOURCE_FILES}
        )

target_link_libraries(OpenGLPractice ${OPENGL_gl_LIBRARY} glfw glm::glm)
