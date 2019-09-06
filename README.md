# CUDA-LIVE
Live-build config files for CUDA-LIVE

``` lb config --bootappend-live "boot=live components modprobe.blacklist=nouveau"; ```

``` lb clean; lb build; ```
### Tested with:

* [ethminer 0.18.0](https://github.com/ethereum-mining/ethminer/releases/tag/v0.18.0)
* [Claymore-Dual-Miner 15.0
](https://github.com/Claymore-Dual/Claymore-Dual-Miner/releases/tag/15.0)
### Troubleshooting
Test shown that on some systems, the onboard GPU(ie: intel) need to be disabled in the BIOS for the Nvidia GPU to boot properly.
