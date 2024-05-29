# Install OpenCV C++

### Install Ubuntu 
On windows run C++ through ubuntu trough wsl, just easier than dealing with mingw/mysys everytime you use a new device. On linux/MacOS install unbuntu so all following steps remain same.

On ubuntu install g++ with `sudo apt-get install g++` then you can run `g++ hello.cpp` to compile a program. Then `./a.out` to run the compiled file.

### Install OpenCV 
[OpenCV docs for installing opencv c++ on ubuntu](https://docs.opencv.org/4.x/d7/d9f/tutorial_linux_install.html):

```
# Install minimal prerequisites (Ubuntu 18.04 as reference)
sudo apt update && sudo apt install -y cmake g++ wget unzip
 
# Download and unpack sources
wget -O opencv.zip https://github.com/opencv/opencv/archive/4.x.zip
unzip opencv.zip
 
# Create build directory
mkdir -p build && cd build
 
# Configure
cmake ../opencv-4.x
 
# Build
cmake --build .
```