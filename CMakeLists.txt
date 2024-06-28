cmake_minimum_required(VERSION 3.22)

project(imgui)

include_directories(
  ${CMAKE_CURRENT_SOURCE_DIR}
  ${CMAKE_CURRENT_SOURCE_DIR}/backends
  ${CMAKE_CURRENT_SOURCE_DIR}/misc/cpp
)

add_library(
  ${PROJECT_NAME} STATIC
  imgui.cpp
  imgui_demo.cpp
  imgui_draw.cpp
  imgui_widgets.cpp
  imgui_tables.cpp
  misc/cpp/imgui_stdlib.cpp
  backends/imgui_impl_glfw.cpp
  backends/imgui_impl_opengl3.cpp
)