---
linkTitle: Compilation 
title: Compilation
weight: 4
---

<!--more-->

After configuring the build, you can compile SpecFWAT using the following command:

```bash
make -j4
```

Following executables will be generated in the `bin` directory:

- `xfwat_mesh_databases` : Generate mesh databases for SPECFEM3D from a ``*.h5`` model file.
- `xfwat_fwd_measure_adj`: Forward modeling, measuring adjoint source, and adjoint simulation.
- `xfwat_post_proc`: Takes sum of kernels, preconditioner, and model regularization.
- `xfwat_optimize`: Get descent direction and update model.