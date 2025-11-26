# DAFART
Deployable Asyncronous Freaking Awesome Receiver and Transmitter

## Summary

D.A.F.A.R.T is a system intended for reliable communications in strenuous communication environments. It is a fully integrated meshing node system that prioritizes critical messages for critical operations.

# OpenWRT Configuration

Firstly you'll need to install OpenWRT for the correct target, this will most likely change depending on which platform you are operating on. 

> D.A.F.A.R.T. is undergoing testing on OpenWRT version `OpenWrt 24.10.2, r28739-d9340319c6`, on the Raspberry PI 4(B) with testing plans for the Qualcomm IPQ601 SoC.

## Prereqs
- [ ] kmod-batman-adv (>=6.6.93.2024.3-r6, <7.0.0) \[Core L2/L3 routing logic\]
- [ ] batctl-full (>=2024.3-r2) \[For improved CLI tooling\]

(for the full list of deps for developers see the DEPENDENCIES\_RPI\_4.md it contains all the neccessary dependencies for D.A.F.A.R.T. to function)

If you do not care to manually install dependencies it is recommend you use the image builder with the accompanying script to generate your image for turn-key operation.


