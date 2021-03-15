# Hackintosh - Opencore EFI for Lenovo M93P


## Specification
| **Component** | **Model** |
| ------------- | --------- |
| CPU | Intel core i3/i5 Haswell |
| Motherboard | Lenovo M93P's mainboard|
| RAM | 8GB (2 x 4GB) Samsung OEM laptop's memory |
| Ethernet | Intel 1GbE |
| OS Disk (Sata3) | Samsung 860 EVO 250GB |

**macOS version**: Bigsur 11.2 (Can be use for 10.15.x also)  

**OpenCore version**: 0.6.2  

**SMBIOS**:  iMac14,4

## How to use
  1. Create directory "EFI" in your EFI partition (e.g. pendrive or hard drive)
  2. Clone this repo and paste directiories "BOOT" and "OC" onto created directory
  3. Download [**GenSMBIOS**](https://github.com/corpnewt/GenSMBIOS) to generate unique SMBIOS information. Run it and select **Generate SMBIOS**, as model select **iMac14,4**.
  4. Open config.plist with [**ProperTree**](https://github.com/corpnewt/ProperTree) and go to PlatformInfo > Generic. Set MLB (Board Serial), SystemSerialNumber (Serial) and SystemUUID (SmUUID) to generated values.
  5. If you are using HD4400 (i3), please add (Key: device-id, Type: Data, Value: 12040000) as image bellow.
  6. Boot it!  

![DeviceProperties a7e57857](https://user-images.githubusercontent.com/8011249/111223563-e33d2a00-860f-11eb-8ebb-02a3de7fc1e8.png)

## Disclaimer

This documentation is published for the sole purpose of learning and tech enthusiasm and with no guarantees of any kind, I’m not responsible of any harm of any kind or loss of data that may occur.
