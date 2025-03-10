# Raylib Project Template using a pre-built raylib dll file and included headers
This project uses a portable .dll file to include raylib functionality. This is how to build and use libraylib.dll:

1. Clone the raylib repository: `git clone https://github.com/raysan5/raylib.git`
2. In VSCode, open the command pallatte with `C+Shift+P` and search CMake: Edit CMake Cache UI
3. Make sure `BUILD_SHARED_LIBS` is set to `ON`
4. Build the raylib library with the CMakeTools extension
5. Copy libraylib.dll from ./build/raylib/
6. Copy all .h files from ./src/ 
7. Setup your CMakeLists.txt file as I have done here. Now you are pointing to the raylib dll and headers and linking them in your project.
8. Note that raylib has a dependency on glfw, however this is dependency is already embedded in the dll file.