file(GLOB HeadFile ${PROJECT_SOURCE_DIR}/utils/*.h)
file(GLOB SourceFile ${PROJECT_SOURCE_DIR}/utils/*.cpp)


add_library(${Library}  ${SourceFile} ${HeadFile})
add_library(Shader GLShader.cpp camera.cpp Terrain.cpp QuadTree.cpp Frustum.cpp Utility.cpp SkyBox.cpp)
add_library(Model ObjModel.cpp)
