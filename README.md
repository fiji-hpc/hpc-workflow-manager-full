# HPC Workflow Manager
## Introduction
This is a bundle of all the projects that are used to build the HPC Workflow Manager.

## Build and installation prerequisites
You will need the following:
* You need a computer with either Windows, Linux or macOS.
* JDK 8, the recommended JDK version is the [Oracle JDK](https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html). If you do not whish to use this distribution you will need to choose one which contains JavaFX.
* JavaFX is used for the GUI, many JDK 8 distributions do not include it by default and a separate installation is necessary for example in OpenJDK.
* [Maven](https://maven.apache.org/) is used to automate the building process.

## Build
Open a terminal window.

Clone this project on your system.
``` bash
git clone --recurse-submodules https://github.com/fiji-hpc/hpc-workflow-manager-full
```

Inside the cloned directory use [Maven](https://maven.apache.org/) with package target to build a jar of this project.
``` bash
mvn clean package
```

## Installation
Follow the these steps to install:
* Download the latest version of Fiji from the [official site](https://fiji.sc/) for your system. Choose the correct version for your operating system.
* Extract the downloaded zip archive anywhere on your system. Fiji is now installed.
* Copy all of the generated jar files found in ```hpc-workflow-manager-full/target/module-assembly-bin/lib``` (of the cloned directory) in the ```plugins``` or ```jars``` directory of Fiji (either directory will do, there is no need to copy to both directories).

HPC Workflow Manager is now ready to be used.

## How to setup the remote cluster for use with HPC Workflow Manager
* If you want to use the parallel Macro and Script features please read the [installation guide](https://github.com/fiji-hpc/Ij1MPIWrapper/blob/master/README.md), and then follow the [short guide](https://github.com/fiji-hpc/Ij1MPIWrapper/wiki/Short-Guide) to get started.
* You may also consider to use the Script (Jython) features along with the [scijava-parallel-mpi](https://github.com/fiji-hpc/scijava-parallel-mpi/wiki/How-to-Install-and-Run) project which provides parallelized common image operations.

### Further information
These Fiji wiki articles were written in the past and some information may be out-of-date.
However they contain relevant information on the design and motivation as well as the SPIMM workflow type which is availabe for use in current versions:
* Click [here](https://imagej.net/SPIM_Workflow_Manager_For_HPC) for an article on the Fiji wiki on the SPIMM Workflow features.
* Click [here](https://imagej.net/HPC_Workflow_Manager) for more information on how to use the Macro parallelization features.
Additinally for more information on one of the ways used to connect to the cluster (middleware):
* [HEAppE Middleware](https://code.it4i.cz/ADAS/HEAppE/Middleware/-/wikis/home) which can be used for SPIMM Workflow type jobs and Macro jobs.
