---
linkTitle: Dependencies
title: Install Dependencies
weight: 2
---

SpecFWAT requires several dependencies to compile and run.

**Required dependencies:**

- Cmake (>= 3.20)
- Fortran compiler (Gfortran >= 11.0 or Intel Fortran >= 19.0)
- MPI (>= 4.0)
- hdf5 (>= 1.10)

**Optional dependencies:**

- CUDA (>= 11.0) for GPU acceleration

{{% callout note %}}
These versions are the minimum required for SpecFWAT that are known to work. Higher versions may be available, and you can use them if you prefer.
{{% /callout %}}


The following sections provide instructions for installing these dependencies on different platforms.

## For personal computers

To install the dependencies for SpecFWAT on your personal computer, we recommend using the [Conda](https://docs.conda.io/en/latest/) package manager. 

{{% steps %}}

### Create a new conda environment

```
conda create -n specfwat
conda activate specfwat
```

### Install dependencies

```bash
conda install -c conda-forge fortran-compiler c-compiler cmake openmpi hdf5
```

{{% /steps %}}

## For supercomputers

To install the dependencies for SpecFWAT on supercomputers, we recommend to load the required modules using the module system.

### N40@BSCC

```bash
module load openmpi/4.1.5_gcc11.2_ucx1.14.1_cuda11.8 cmake/3.30.0 cuda/11.8 hdf5/1.13.3
```

### Niagara@CCDB

```bash
module --force purge
module load NiaEnv/2022a intel intelmpi hdf5 netcdf cmake
```
