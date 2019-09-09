# CUDA-LIVE
Config Files for creating [Live](https://live-team.pages.debian.net/live-manual/html/live-manual/about-project.en.html#76) Debian(buster) bootable ISO for CUDA-9.x(Nvidia)

### Features
* nvidia-driver
* nvidia-cuda-toolkit
* lxde-core
* boinc-client-nvidia-cuda
* boinc-manager

### Requirement
* [CUDA-Enabled](https://developer.nvidia.com/cuda-gpus#compute) GPU[s] supported by CUDA-9.x(Nvidia)
* git
* live-build

``` sudo apt-get update;```

``` sudo apt-get install git live-build;```

### Installation methods

1. (recommended) ``` git clone https://github.com/yanicky/CUDA-LIVE; cd CUDA-LIVE;```
``` ```
2. (other) ``` mkdir CUDA-LIVE; cd CUDA-LIVE; lb config --config=https://github.com/yanicky/CUDA-LIVE```

### Building the bootable ISO image
use the following commands in the base directory to build the iso

```sh auto/config; sudo lb clean; sudo lb build;```

Creating a iso file named live-image-amd64.hybrid.iso of about 2GB.

### Tested For [CUDA](https://developer.nvidia.com/cuda-zone) parallel computing with:
* [Boinc](https://boinc.berkeley.edu/) (included)
* [ethminer 0.18.0](https://github.com/ethereum-mining/ethminer/releases/tag/v0.18.0) for CUDA-9 (not included)
* [Claymore-Dual-Miner 15.0
](https://github.com/Claymore-Dual/Claymore-Dual-Miner/releases/tag/15.0) (not included)

### Troubleshooting
* (UEFI)Secure Boot need to be disabled since it's not configured in the live-build config and will require user bios configuration to work.
* (nvidia-driver)Test shown that on some systems, the onboard GPU(ie: intel) need to be disabled in the BIOS for the Nvidia GPU to boot properly.
