# Installation in Linux: Compile OpenCV (>= 3.0)

## Download files

Install minimal prerequisites 

```shell
sudo apt update && sudo apt install -y cmake g++ wget unzip git-all
```

You could clone the github repositories (git).

```shell
git clone https://github.com/opencv/opencv.git
git clone https://github.com/opencv/opencv_contrib
```

Or download and unpack the zips (wget).

```shell
wget -O opencv.zip <https://github.com/opencv/opencv/archive/4.x.zip>
wget -O opencv_contrib.zip <https://github.com/opencv/opencv_contrib/archive/4.x.zip>
unzip opencv.zip
unzip opencv_contrib.zip
```

## Building and Installing

Create build directory and switch into it

```shell
mkdir -p build && cd build
```

Configure

```shell
cmake -DOPENCV_EXTRA_MODULES_PATH=../opencv_contrib/modules ../opencv
```

Build

```shell
cmake --build .
```

Run compilation process

```shell
make -j4
```

Finally, install

```shell
sudo make install
```

## Sources

- [Installation in Linux](https://docs.opencv.org/4.x/d7/d9f/tutorial_linux_install.html)
