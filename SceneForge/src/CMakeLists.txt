
set(SOURCES
        main.cpp
)

add_executable(SceneForge ${SOURCES})
find_package(Vulkan)
target_link_libraries(SceneForge glm_static glfw imgui Vulkan::Vulkan)


