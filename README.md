# Opencore EFI for Asus B460i Strix Motherboard


## Version


| Item | Version |
| -------- | --------------- |
| MacOS    | Monterey 12.2.1 |
| Opencore | 0.7.8           |

## Hardware

- 主板: Asus ROG STRIX B460-I
- WiFi: 主板自带AX200
- 蓝牙: 主板自带
- CPU: Intel Core i7-10700
- GPU: Intel UHD630
- 声卡: 主板自带ALCS1220A

## Notice

- Monterey与FackPCIID*不兼容，会造成随机内核崩溃，及关机时必定崩溃
- Monterey中，Intel蓝牙使用IntelBluetoothFirmware.kext和BlueToolFixup.kext
- AX200使用AirportItlwm.kext，开启SecureBoot，参考https://www.mfpud.com/topics/3403/
- 在Device Properties中无需添加声卡，添加后设置错了反而会导致声卡失效
- Monterey需要定制USB，并且取消勾选XhciPortLimit。不过不定制也能用。