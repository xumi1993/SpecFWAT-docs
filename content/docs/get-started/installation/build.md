---
linkTitle: Configuration 
title: Configuration
weight: 30
---

<!--more-->

SpecFWAT is built using CMake, a cross-platform build system. The following instructions will guide you through the process of building SpecFWAT on your system.

{{% steps %}}

### Create a build directory

```bash
mkdir build && cd build
```

### configure the build

Bascially, you can use the following command to configure the build:

```bash
cmake ..
```

{{% /steps %}}


### More options

#### 1. Specify Compilers:
If you have multiple compilers installed, you can specify the Fortran and C compilers using the `FC` and `CC` options, respectively. For example on **Niagara@CCDB**:

```bash
CC=icc CXX=icpc FC=mpifort MPIFC=mpifort cmake ..
```

More options can be specified in the `cmake` command. For example, you can specify the HDF5 directory and enable GPU support. Here are some common options:

#### 2. Specify the HDF5 directory:
If the hdf5 library is not installed in library path, you can specify its path using the `HDF5_ROOT` option. For example:

```bash
cmake -DHDF5_ROOT=/path/to/hdf5 ..
```

#### 3. Enable GPU support:

Currently, SpecFWAT only supports CUDA for GPU acceleration. The CUDA architecture can be specified using the <code>CUDA_ARCH</code> option. Check the table below for the supported architectures:

| CUDA_ARCH | Architecture | Example Card |
|-----------|--------------|--------------|
| 0 (default) | GPU on current machine | N/A |
| 4 | Tesla | K10, Geforce GTX 650 |
| 5 | Kepler | K20 |
| 6 | Kepler | K80 |
| 7 | Maxwell | Quadro K2200 |
| 8 | Pascal | P100 |
| 9 | Volta | V100 |
| 10 | Turing | GeForce RTX 2080 |
| 11 | Ampere | A100 |
| 12 | Hopper | H100 |

For example, to enable CUDA support and set the architecture to Ampere (A100), you can use the following command:

```bash
cmake -DUSE_CUDA=on -DCUDA_ARCH=11 ..
```

