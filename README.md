# MonaServer
===========

**MonaServer** is a new Web server born from the [Cumulus](https://github.com/OpenRTMFP/Cumulus) project.

In addition to **RTMFP** it includes **RTMP/RTMPE**, **WebSocket**, **HTTP**, a **NoDB** system and a lot of improvements.

# 1.Binaries & Build
## 1.1.Windows

A [32-bit Windows zipped package](https://sourceforge.net/projects/monaserver/files/MonaServer_Win32.zip/download) is provided to quickly test MonaServer.

**Note :** In order to use it you need the [C++ Redistributable Packages for Visual Studio 2013](http://www.microsoft.com/en-us/download/details.aspx?id=40784).

We recommend you to clone the github version from the sources and to follow the [Installation instructions](http://www.monaserver.ovh/installation.html) for production use.


## 1.2.Linux

Make sure you installed g++, gcc, make, libssl-dev
Dependencies Validation:
```
g++ -v
gcc -v
make -v
```
Dependencies Installation:
```
apt insatll g++
apt install gcc
apt insatll make
apt install libssl-dev
```
Luajit and MonServer Installation
```
git clone https://github.com/panhavad/monaserver
git submodule update --init --recursive

cd monaserver/luajit-2.0
make
make install
luajit -v

cd ..
make

cd MonaServer
./MonaServer
```

### Reference:
1. https://luajit.org/install.html
2. https://www.monaserver.ovh/installation.html#build



