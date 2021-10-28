# open-ondemand-apps

## Introduction

[Open-Ondemand](https://osc.github.io/ood-documentation/latest/) provides a convenient interface for users to access remote servers such as HPC systems.

This repository will store the versions as running on [Supercomputing Wales](https://portal.supercomputing.wales) Hawk system.

## Rstudio

Using Rocker container this spins up a Rstudio session.  See Singularity file.

## Jupyter

Uses Anaconda as installed on Hawk to provide Jupyter session.  If users install jupyter in their environments installed in home directory then the kernels for their environments also appear as an option.

## bc_desktop

To allow remote desktop a container was created to allow the desktop (Mate in this case from EPEL) dependencies to be isolated from host OS which doesnt allow EPEL repository.  This also supports VirtualGL and TurboVNC to provide 3D interface.  Requires Slurm configurationt to support spinning up Xorg and provide a desktop.
