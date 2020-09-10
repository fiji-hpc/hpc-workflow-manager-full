# HPC Workflow Manager
## Introduction
This is a bundle of all the projects that are used to build the HPC Workflow Manager.

## Build
Clone this project on your system.
Use maven with package target to build a jar of this project.

## Installation
You need a computer with either Windows, Linux or macOS.

### Follow the these steps to install:
* Download the latest version of Fiji from the [official site](https://fiji.sc/) for your system. Choose the correct version for your operating system.
* Extract the downloaded zip archive anywhere on your system. Fiji is now installed.
* Copy all of the generated jar files found in hpc-workflow-manager-full/target/module-assembly-bin/lib (of the cloned directory) in the "plugins" or "jars" directory of Fiji (either directory will do, there is no need to copy to both directories).

HPC Workflow Manager is now ready to be used.
If you want to use the parallel Macro and Script features please read the [installation guide](https://github.com/MKrumnikl/Ij1MPIWrapper/blob/master/README.md), and then follow the [short guide](https://github.com/MKrumnikl/Ij1MPIWrapper/wiki/Short-Guide) to get started.
You may also consider to use the Script features along with the [scijava-parallel-mpi](https://github.com/fiji-hpc/scijava-parallel-mpi/wiki/How-to-Install-and-Run) project which provides parallelized common image operations.

### Further information
Click [here](https://imagej.net/SPIM_Workflow_Manager_For_HPC) for an article on the Fiji wiki on the SPIMM Workflow features.
Click [here](https://imagej.net/HPC_Workflow_Manager) for more information on how to use the Macro parallelization features.