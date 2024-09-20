# Learning CMake
In this repo, I'll implement a small project using CMake to create libraries and use it. 
The tree folder is:
```
D:. 
│   CMakeLists.txt 
│   main.cpp
│   
├───MyLib
│       CMakeLists.txt
│       MyLib.cpp
│       MyLib.h
│       
└───printlib
        CMakeLists.txt
        print.cpp
        print.h
```
In this project, I will implement an easy project that included of an executable file `main.cpp`. This file include MyLib and use a function this library. 
Then, MyLib uses the function in printlib to implement the print() function (I am declaring `STATIC` library, it will be built as .lib library in the end).

To run this project, please stay at the folder with the same level with top-level CMakeLists.txt.
Then, run those commands in terminal:
```
cmake -S . -B ./build
cd build
cmake --build .
```

Right now, we can navigate to the Debug folder in build directory, then run the ./myapp.exe to run.
