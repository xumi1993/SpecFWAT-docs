---
linkTitle: Download
title: Download Source Code
weight: 10
---

Users are available to access source code from Github repository. To download the source code, you can use the following command:

```bash
git clone https://github.com/CompSeismoUT/SpecFWAT.git
```

Two submodules are required to run SpecFWAT, namely `SpecFEM3D` and `yaml-cpp`. They will be automatically fetched when you build the SpecFWAT. Alternatively, you can also download them separately using the following commands:

```bash
git clone --recursive https://github.com/CompSeismoUT/SpecFWAT.git
```

{{% callout note %}}
The url of submodules are recorded in the `.gitmodules` file. You can also modify them to point to your own fork of the repository.
{{% /callout %}}