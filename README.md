# [OpenCore](https://github.com/acidanthera/OpenCorePkg) configuration for MSI B550M MORTAR

**macOS ：11.6**

**SMBIOS : MacPro7,1**

### Builds

| **Component** | **Model**                  |
| ------------------- |----------------------------|
| CPU                 | AMD R7 5800X               |
| Motherboard         | MSI B550M MORTAR WIFI |
| RAM                 | 16GB x 2          |
| Audio Chipset       | ALCS1200A                  |
| GPU                 | RX 6800                    |
| Ethernet            | RTL8125B 2.5GbE            |
| WiFi & Bluetooth    | Intel WiFi 6 AX200         |

### What works

- Audio
- Ethernet
- USB
- Wi-Fi
- Bluetooth

### Read Me First!

- This config adopts the RX 6800 and it's [Smart Access Memory](https://www.amd.com/en/technologies/smart-access-memory)
  by default, you need to enable `Resizeable Bar` and `Above 4g memory` properties in BIOS.
- If your cpu don't have 8 cores (e.g. 6 core 5600X)_,_ you must change patch values
  of `algrey - Force cpuid_cores_per_package` to boot your system.
  See [AMD_Vanilla ReadMe](https://github.com/AMD-OSX/AMD_Vanilla#read-me-first) for details.

### Monterey

Most MSI B550 motherboard need use the 7C94v12 version of the bios to start Monterey. Please test yourself according to
your hardware.
