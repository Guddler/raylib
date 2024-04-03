This branch is forked from Raylib tag v4.5 in order to work on a port for Amiga OS4.1

### How to compile

Install GLFW from Clib4 repository:

`sudo apt install libglfw3-clib4`

Then create a build dir:

`mkdir build`

Enter int build dir and execute cmake:

```
cd build
cmake -DCMAKE_TOOLCHAIN_FILE=<YourClib4Toolchain> -DPLATFORM=AOS4 -DBUILD_EXAMPLES=OFF -DCMAKE_BUILD_TYPE=Release -DUSE_EXTERNAL_GLFW=ON ..
make
```

An example of a cmake toolchain for AmigaOS4 can be found here:

[https://github.com/afxgroup/clib4-cmake-toolchain](https://github.com/afxgroup/clib4-cmake-toolchain)
