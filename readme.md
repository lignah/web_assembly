# c to webassembly

<!-- <img src="/​/thumbnail.png" style="pointer-events: none;"> -->
[![](/​/thumbnail.png)](https://lignah.github.io/web_assembly/)

**click the image to link**


```
$ option)
$ pacman -S python
$ mkdir -p /tmp
```

```
lignah@DESKTOP-XRKAFN8 MSYS ~/web_assembly
$ git clone https://github.com/emscripten-core/emsdk.git
```

```
$ cd emsdk
$ ./emsdk install latest
$ ./emsdk activate latest
$ source ./emsdk_env.sh
```

```
lignah@DESKTOP-XRKAFN8 MSYS ~/web_assembly/emsdk
$ cd ..
```


```
lignah@DESKTOP-XRKAFN8 MSYS ~/web_assembly
$ vim <filename>.c
$ ls
<filename>.c  emsdk
```

```
$ emcc <filename>.c -o <filename>.js -s EXPORTED_FUNCTIONS="['_<function_name>']" -s MODULARIZE -Os --no-entry
```