<img src="https://github.com/christiansiewert/rooster/raw/rooster/docs/logo.jpg" />

# Rooster

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/christiansiewert/rooster)

This is the develop branch of [rooster] and a complete reimplementation of [cmangos/classic].

[rooster]: https://github.com/christiansiewert/rooster/tree/rooster
[cmangos/mangos-classic]: https://github.com/cmangos/mangos-classic

## Build example

### Configure

`cmake ../SRC_DIR/ -DCMAKE_INSTALL_PREFIX=\../SRC_DIR/run -DBUILD_EXTRACTORS=ON -DPCH=1 -DDEBUG=0 -DBUILD_PLAYERBOT=ON`