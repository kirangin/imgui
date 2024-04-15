project(imgui-docking)

set(CMAKE_CXX_STANDARD 17)

include_directories(
  ${CMAKE_CURRENT_SOURCE_DIR}
  ${CMAKE_CURRENT_SOURCE_DIR}/backends
  ${CMAKE_CURRENT_SOURCE_DIR}/include
)

add_library(
  imgui
  STATIC
  imgui.cpp
  imgui_demo.cpp
  imgui_draw.cpp
  imgui_widgets.cpp
  imgui_tables.cpp
  backends/imgui_impl_glfw.cpp
  backends/imgui_impl_opengl3.cpp
  misc/cpp/imgui_stdlib.cpp
)