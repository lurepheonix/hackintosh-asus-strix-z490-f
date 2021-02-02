# Hackintosh based on ASUS ROG STRIX Z490-F

## Configuration
### Hardware
| Device      | Model                                        |
| ----------- | -------------------------------------------- |
| CPU         | Intel Core i5-10600K                         |
| Motherboard | ASUS ROG STRIX Z490-F GAMING                 |
| RAM         | Kingston HyperX Fury Black 3733 MHz 16gb * 2 |
| Video card  | Sapphire RX 580 Nitro 4GB                    |
| Case        | Thermaltake Commander G32                    |

### Software
- Bootloader: OpenCore 0.6.5
- OS: macOS Big Sur 11.1
- OS (old): macOS Catalina 10.15.7
### BIOS settings
**Note:** some settings are different from OpenCore guide.
#### Disable
- Fast Boot
- Serial/COM port
- Intel SGX

#### Enable
- VT-d
- VT-x
- CSM
- Above 4G decoding
- EHCI/XHCI hand-off

#### Set
- Secure Boot: set OS type to Other OS
#### Leave as is
- CFG lock: no such option, already unlocked

### Working
- [x] CPU/Motnerboard
- [x] Integrated graphics [Intel UHD 630]
- [x] Discrete graphics [Radeon RX 580]
- [x] Audio [Realtek ALCS1220A]
- [x] Intel i225-V Ethernet (with kext)
- [x] Shutdown/restart
- [x] Sleep/wake
- [x] USB
- [x] Power management
- [X] Docker
- [x] etc
### Not working
- Intel UHD 630 output (likely a problem with HDMI output, DP should work, didn't fix)