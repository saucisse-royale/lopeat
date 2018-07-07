# lopeat
Minimalist step sequencer and synthesizer

## Building
You need to install [libsndfile](http://www.mega-nerd.com/libsndfile/) and [Soundpipe](https://github.com/PaulBatchelor/Soundpipe) before `go get`-ing.

### MinGW-w64 on MSYS2
```shell
pacman -Sy mingw-w64-x86_64-libsndfile
wget https://github.com/PaulBatchelor/Soundpipe/archive/v1.7.0.tar.gz
tar xfz https://github.com/PaulBatchelor/Soundpipe/archive/v1.7.0.tar.gz
cd Soundpipe-1.7.0
make
PREFIX=/mingw64 make install
```

Then, simply run:
```shell
go get github.com/saucisse-royale/lopeat
go install github.com/saucisse-royale/lopeat
lopeat
```
