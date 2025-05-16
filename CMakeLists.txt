# CMake最低版本要求
cmake_minimum_required(VERSION 3.10)

# 项目名称和版本号
project(MyProject VERSION 1.0)

# 设置C++标准
set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# 添加可执行文件
add_executable(${PROJECT_NAME} 
    main.c
)

# 查找并包含子目录中的CMakeLists.txt，如果有的话
# add_subdirectory(src)

# 如果有第三方库，可以在这里添加查找路径或链接库
# find_package(SomeLibrary REQUIRED)
# target_link_libraries(${PROJECT_NAME} SomeLibrary::SomeLibrary)

# 安装设置（可选）
# install(TARGETS ${PROJECT_NAME} DESTINATION bin)