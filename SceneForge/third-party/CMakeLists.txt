
set(GLFW_BUILD_EXAMPLES OFF CACHE BOOL "Turn off GLFW build stuff")
set(GLFW_BUILD_TESTS OFF CACHE BOOL "Turn off GLFW build stuff")
set(GLFW_BUILD_DOC OFF CACHE BOOL "Turn off GLFW build stuff")
add_subdirectory(glfw)

set(GLM_TEST_ENABLE  OFF CACHE BOOL "En/Disable GLM tests")
add_subdirectory(glm)
target_include_directories(glm_static PUBLIC glm/)

add_library(imgui INTERFACE)
target_include_directories(imgui INTERFACE imgui/)