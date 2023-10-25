# Lab1
    The paths used by target_sources and target_include_directories are relative to: These paths are typically relative to the location of your CMakeLists.txt file. For example, if you specify target_sources(hello_world PRIVATE src/hello.cpp), it means that src/hello.cpp is located in the same directory as your CMakeLists.txt. Similarly, target_include_directories(hello_world PRIVATE include) tells CMake to include header files from the include directory relative to your CMakeLists.txt.

    Differences between CMake and Ninja:
        CMake is a meta-build system that generates build systems for various platforms and compilers (like Makefiles or Ninja build files). It's responsible for generating the necessary build files but isn't used for the actual building of the project.
        Ninja is a build system like Make, but it's designed to be faster and is often used as the actual tool for compiling and linking the code. In CMake, you can specify that you want to generate Ninja build files, and then you use Ninja to build the project.

    Importance of running CMake in its own directory: It's important to run CMake in its own directory to keep the generated build system files and object files separate from your source code. This separation ensures that your source code remains clean and that you can easily clean, rebuild, or change build systems without affecting your source files. It's a good practice for maintaining a clean and organized project structure.
