# libretro-crocods

Look for .kcr file format to use CrocoDS at its best: https://github.com/redbug26/crocods-core/wiki/kcr

BUILD INSTRUCTIONS:

``` 
git clone https://github.com/redbug26/libretro-crocods.git
cd libretro-crocods/
git submodule update --init --recursive
``` 

Compile for osX
``` 
make -f Makefile.libretro platform="osx" -j2 CC="cc" CXX="c++"
```

Compile for linux
``` 
make -f Makefile.libretro platform="linux" -j2 CC="cc" CXX="c++"
```

Compile for win
``` 
make -f Makefile.libretro platform="win" -j2 CC="cc" CXX="c++"
```

Compile for raspberry
```
sudo apt-get install gcc-arm-linux-gnueabi make ncurses-dev g++-arm-linux-gnueabi
make -f Makefile.libretro platform="unix" -j2 CC="arm-linux-gnueabi-gcc" CXX="arm-linux-gnueabi-g++"
```

