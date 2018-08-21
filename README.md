## Building DeepWebCoin

### On linux:

Dependencies: GCC 4.9 or later, CMake 2.8.6 or later, and Boost 1.55.
You may download them from:

* http://gcc.gnu.org/
* http://www.cmake.org/
* http://www.boost.org/

Alternatively, it may be possible to install them using a package manager.

```
git clone https://github.com/deepwebcoin/deepwebcoin.git
export CXXFLAGS="-std=gnu++11"
cd deepwebcoin
mkdir build && cd build
cmake -DCMAKE_BUILD_TYPE=Release .. && make
```

The resulting executables can be found in build/release/src.


### On Windows:
Dependencies: MSVC 2013 or later, CMake 2.8.6 or later, and Boost 1.55. You may download them from:
* http://www.microsoft.com/
* http://www.cmake.org/
* http://www.boost.org/

To build, change to a directory where this file is located, and run this commands:

```
md build && cd build
cmake -G "Visual Studio 12 Win64" .. -DCMAKE_BUILD_TYPE=Release
MSBuild deepwebcoin.sln /p:Configuration=Release /m
```

Good luck!
