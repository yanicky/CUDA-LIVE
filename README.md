# CUDA-LIVE
Live-build config files for CUDA-LIVE

``` lb config --bootappend-live "boot=live components modprobe.blacklist=nouveau"; ```

``` lb clean; lb build; ```

### Troubleshooting
Test shown that on some systems, the onboard GPU(ie: intel) as to be disabled in the BIOS for the Nvidia GPU to boot properly.
