# Imgui Cmake Starter
## notice
**only tested on windows and wsl**

**all libs built from source**

**this starter project use opengl3 and sdl2 as imgui's backends， and ourown diretory uses the corresponding example from imnode*

## how to build
following commads will make debug target bydefault

~~~shell
cd ImguiCmakeStarter
mkdir cmake_build
cmake -S . -B .\cmake_build\
cmake --build .\cmake_build\ 
~~~~

Also can intall it, default intall path is "${CMAKE_CURRENT_SOURCE_DIR}/install", you can check it in CmakeLists.txt.  

Note we should use --config Debug option here, because cmake intall command find Release target by default but we complie the Debug one only

~~~shell
cmake --install .\cmake_build\ --config Debug 
~~~
If you want intall it at another dir, just modify the default intallation path in CmakeLists.txt, or overrite it in command line option using `-DINSTALL_PREFIX="custom_install"`
