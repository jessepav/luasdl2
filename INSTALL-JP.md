This is how I built and installed the library:

```
mkdir build
cd build
cmake -DCMAKE_INSTALL_PREFIX=/opt/luasdl2 \
      -DWITH_LUAVER=JIT -DLuaJIT_INCLUDE_DIR=/usr/local/include/luajit-2.1/ \
      ..
make
make install
```

Note the case of `LuaJIT_INCLUDE_DIR`, which is different from the case as
described in `INSTALL.md`.
