# CS455/555 Opencv Install

## Linux:
install cmake: 
```
sudo apt-get -y install cmak
```
[download opencv4.4.0](https://sourceforge.net/projects/opencvlibrary/files/4.4.0/OpenCV%204.4.0.zip/download)  
unzip opencv-4.4.0, then
```
cd opencv-4.4.0
mkdir build 
cd build
```
```
sudo apt-get install build-essential
sudo apt-get install cmake git libgtk2.0-dev pkg-config libavcodec-dev libavformat-dev libswscale-dev
```

```
cmake -D CMAKE_BUILD_TYPE=Release -D -DOPENCV_GENERATE_PKGCONFIG=ON CMAKE_INSTALL_PREFIX=/usr/local ..
make -j8
sudo make install
sudo ldconfig
```
## MacOS:
install xcode (search xcode in Apple App Store)
```
sudo xcode-select --install
```
install homebrew: 
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
```
brew install pkg-config
brew install opencv@4
```

## Verify
```
pkg-config --cflags --libs opencv4
```


