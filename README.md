# Dell-Latitude-3410_Hackintosh
OpenCore EFI for Dell Latitude 3410 with 10th generation Intel processor

## Hardware Info
|  Type  |  Model  |
|  :----  |  :----  |
|  CPU  |  Intel Core i7-10510U  |
|  iGPU  | Intel UHD620  |
|  dGPU  | ~~NVIDIA GeForce MX230~~ (Disabled)  |
|  Storage  | SK hynix BC511 NVMe SSD  |
|  Audio  | Realtek ALC236  |
|  WLAN  | Intel AX201  |
|  LAN  | Realtek RTL8111  |

## macOS version

Build for macOS Sonoma 14.0, should also work for other lower versions of macOS  
If you need to use it for other versions of macOS besides Ventura, please change `AirportItlwm.kext` in `EFI/OC/Kexts` to the corresponding version  
e.g. Download and use `AirportItlwm_v2.2.0_stable_BigSur.kext.zip` from [this link](https://github.com/OpenIntelWireless/itlwm/releases) for macOS 11


## Not working
dGPU (No NVIDIA dGPU support)  
Microphone (No Intel microphone array support, use USB-C DAC instead)  
Sleep (AOAC, Not stable enough to enable)  
Display Port via Type-C not tested yet  

## Remark
Modify SMBIOS info in `EFI/OC/config.plist/Root/PlatformInfo/Generic` before boot  
Check [here](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/coffee-lake-plus.html#platforminfo) for more help
