cmake_minimum_required(VERSION 3.7)
project(3d-viewer-tool)

set(CMAKE_CXX_STANDARD 11)

set(CXX_PROPERTIES "-fPIC")
set(CMAKE_CXX_FLAGS "${CMAKE_COMPILE_FLAGS} ${CXX_PROPERTIES}")
set(SOURCE_FILES
        "src/World Objects/Polygon.cpp"
        "src/World Objects/Vertex.cpp"
        "src/World Objects/WorldObject.cpp"
        "src/World Objects/Mesh.cpp"
        "src/World Objects/Axis.cpp"
        "src/Template Objects/TemplateObjects.cpp")
set(HEADERS
        "src/World Objects/WorldObject.h"
        "src/World Objects/Axis.h"
        "src/World Objects/Mesh.h"
        "src/Template Objects/TemplateObjects.h")
add_executable(opengl-debugger opengl_debugger_utility.cpp ${SOURCE_FILES} ${HEADERS})
set_target_properties(opengl-debugger PROPERTIES COMPILE_FLAGS ${CXX_PROPERTIES})
target_link_libraries(opengl-debugger -lGL -lglut)