# Ryzentosh EFI configuration

This repo contains my EFI configuration used to boot macOS on a custom PC using OpenCore.

## PC specs

| Part        | Name                                     |
| ----------- | ---------------------------------------- |
| Motherboard | Gigabyte B550 Aorus Elite AX v2          |
| CPU         | AMD Ryzen 5 5600X                        |
| GPU         | Sapphire Pulse Radeon 5700XT             |
| RAM         | Crucial Ballistix DDR4 3600 MHz (8GB x2) |
| Storage     | Sabrent Rocket NVMe PCIe 4.0 (500 GB)    |
| Ethernet    | Realtek RTL8125 2.5GbE                   |
| Wi-Fi & BT  | Intel Wi-Fi 6 AX200 (MoBo bundled)       |

### Notes

- NVMe storage appeared as external drive. Resolved adding a new item inside _DeviceProperties_ section in _config.plist_ file.
- Using _AirportItlwm_ kernel extension Handoff and Universal Clipboard works correctly. Using Airdrop the device will be visibile to others but unable to connect and send/receive files.
