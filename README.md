# CUDAInstallation
Notes on installing CUDA on Debian Bullseye.

## For now, CUDA is installed without GPUDirect Storage installed.
If this is to be installed later:
- iommu is not available, and is thus disabled (which it must be for GPUDirect)

## The nouvea driver is not installed:

`sudo lsmod | grep nouveau` gives no result.
