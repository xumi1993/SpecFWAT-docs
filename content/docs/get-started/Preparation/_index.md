---
linkTitle: Preparation
title: Preparation
weight: 1
sidebar:
  open: true
---

## Project Structure

The SpecFWAT project is organized based on Specfem3D. Thus, subdirectories of Specfem3D are inherited in SpecFWAT. New directories of input files `fwat_data` and `src_rec` are added to the SpecFWAT project. The following is a brief description of the directory structure of a project:


```
- Project
  ├── DATA
  │   ├── Par_file
  │   ├── fwat_params.yml
  │   ├── meshfem3D_files
  │   |   ├── Mesh_Par_file.noise
  │   |   ├── Mesh_Par_file.tele
  │   |   ├── interfaces.noise.dat
  │   |   ├── interfaces.tele.dat
  │   |   ├── topo1.dat
  │   |   ├── topo2.dat
  │   |   ├── ...
  ├── fwat_data
  │   ├── event1
  │   │   ├── net.sta.BXZ.sac
  │   │   ├── net.sta.BXR.sac
  │   │   ├── ...
  │   ├── event2
  │   │   ├── net.sta.BXZ.sac
  │   │   ├── net.sta.BXR.sac
  │   │   ├── ...
  │   ├── ...
  ├── src_rec
  │   ├── FKmodel_event1
  │   ├── FKmodel_event2
  │   ├── ...
  │   ├── FORCESOLUTION_event3
  │   ├── FORCESOLUTION_event4
  │   ├── ...
  |   ├── STATIONS_event1
  │   ├── STATIONS_event2
  │   ├── ...
  |   ├── sources_noise.dat
  │   ├── sources_tele.dat
  └── bin
```