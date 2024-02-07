# CUDAInstallation
Notes on installing CUDA and NVIDIA GPU drivers on Debian Bullseye.

## For now, CUDA is installed without GPUDirect Storage installed.
If this is to be installed later:
- `iommu` is not available, and is thus disabled (which it must be for 
GPUDirect). In fact, there seems to be no IOMMU hardware available on 
the system.

## CUDA installation

Follow the instructions at [https://developer.nvidia.com/cuda-downloads](https://developer.nvidia.com/cuda-downloads).

The nouveau driver is not installed: `sudo lsmod | grep nouveau` gives no result.

The open kernel module flavour didn't work for me. Use the legacy 
kernel module flavour: '$ sudo apt-get install -y cuda-drivers'.
