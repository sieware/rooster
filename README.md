<img src="https://raw.githubusercontent.com/christiansiewert/rooster/rooster-develop/docs/logo.jpg" />

# Rooster

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/sieware/rooster)

This is the develop branch of Rooster and a complete reimplementation of the [cmangos] backend emulators.

## Directory structure

- **bin/** - shell scripts or something similar
- **build/** - output directory for build artifacts
- **docs/** - documentation 
- **src/** - sourcecode
  - **src/databases/** - setup and/or sql files for creating our databases
  - **src/server/** - sourcecode for our server backends (vanilla, tbc, wotlk, etc.)

We'll try to handle each database and backend server as a separate repository so we can inject those as a git submodule.

## Build example

### Configure

```
cd build/
cmake ../src/ -DCMAKE_INSTALL_PREFIX=\../src/run -DBUILD_EXTRACTORS=ON -DPCH=1 -DDEBUG=0 -DBUILD_PLAYERBOT=ON
make
make install
```

[cmangos]: https://github.com/cmangos
