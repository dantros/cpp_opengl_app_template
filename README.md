# C++ OpenGL App Template

Basic C++ project configuration to start a simple OpenGL based application.

It includes a minimal setup with the following libraries:
- OpenGL 3.3 via glad
- GLFW3
- glm
- Dear ImGui
- argparse
- json
- spdlog
- whereami2cpp

CMake is used as build system and it should work out of the box.

`main.cpp` includes a working code using all libraries.

## Quick start

You can start by clicking 'Use this template' at the upper right corner of the Github website. You will get a clone of this repo in your repositories to start working.

After making a local clone, you need to initialize and update the git submodules by executing at the root of the repository:
```
git submodule update --init --recursive
```
Once you are done, you can generate the build files with cmake presets.
```
cmake --presets ninja-release
```
And then, just go to `../build_cmake/ninja-release/` and execute `ninja` and you will get your binary file.
You can also get a Visual Studio solution file for your convenience, check [CMakePresets.json](CMakePresets.json) file.

You should have [cmake](https://cmake.org/), [ninja](https://ninja-build.org/) and a compiler such as [Visual Studio Community](https://visualstudio.microsoft.com/vs/community/) availables in your development environment.
