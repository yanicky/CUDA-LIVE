# CUDA-LIVE
Config Files for creating Live-build Debian(stretch) bootable ISO for CUDA-8.x(Nvidia)

```sh auto/config; lb clean; lb build; ```

### Features
* boinc-client-nvidia-cuda
* boinc-manager
### Tested For CUDA Mining with:
* [Boinc](https://boinc.berkeley.edu/)
* [ethminer 0.18.0](https://github.com/ethereum-mining/ethminer/releases/tag/v0.18.0) for CUDA-8
* [Claymore-Dual-Miner 15.0
](https://github.com/Claymore-Dual/Claymore-Dual-Miner/releases/tag/15.0)
### Troubleshooting
* (UEFI)Secure Boot need to be disabled since it's not configured in the live-build config and will require user bios configuration to work.
* (nvidia-driver)Test shown that on some systems, the onboard GPU(ie: intel) need to be disabled in the BIOS for the Nvidia GPU to boot properly.
