# pmemd-pmf-build
Utilities for testing and building of the [pmemd-pmf](https://github.com/kulhanek/pmemd-pmf) package.

## pmemd-pmf Features:
* modified version of pmemd from [AMBER](https//ambermd.org)
* integration with [PMFLib](https://github.com/kulhanek/pmflib)

## Building and Installation

### Testing Mode
```bash
$ git clone --recursive https://github.com/kulhanek/pmemd-pmf-build.git
$ cd pmemd-pmf-build
$ ./build-utils/00.init-links.sh
$ ./01.pull-code.sh
$ ./04.build-inline.sh   # build the code inline in src/
```

### Production Build into the Infinity software repository
```bash
$ git clone --recursive https://github.com/kulhanek/pmemd-pmf-build.git
$ cd pmemd-pmf-build
$ ./build-utils/00.init-links.sh
$ ./01.pull-code.sh
$ ./10.build-final.sh
```

### Production Build into Custom Directory
```bash
$ git clone --recursive https://github.com/kulhanek/pmemd-pmf-build.git
$ cd pmemd-pmf-build
$ ./build-utils/00.init-links.sh
$ ./01.pull-code.sh
$ cmake -DCMAKE_INSTALL_PREFIX=/path/to/pmemd-pmf/installation/directory
$ make
$ make install
```

