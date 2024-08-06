cmake_minimum_required(VERSION 3.20)
set(CMAKE_LEGACY_CYGWIN_WIN32 OFF)

project(cpp_opengl_app_project CXX)

add_subdirectory("third_party/whereami2cpp")
add_subdirectory("third_party/glad")
add_subdirectory("third_party/glfw")
add_subdirectory("third_party/imgui_cmake")

add_executable(cpp_opengl_app "source/main.cpp")
set_property(TARGET cpp_opengl_app PROPERTY CXX_STANDARD 20)
target_include_directories(cpp_opengl_app PRIVATE
    "third_party/argparse/include"
    "third_party/whereami2cpp/source"
    "third_party/spdlog/include"
    "third_party/json/include"
    "third_party/glad/include"
    "third_party/glfw/include"
    "third_party/glm/include"
    "third_party/imgui"
)
target_link_libraries(cpp_opengl_app PRIVATE whereami2cpp glad glfw imgui)
