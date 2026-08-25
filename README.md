# Device tree for Xiaomi Mi 8 SE (codenamed _"sirius"_)

==================================

## Device specifications

Basic   | Spec Sheet
-------:|:-------------------------
SoC     | Qualcomm SDM710 Snapdragon 710 (10nm) 
CPU     | Octa-core (2x2.2 GHz Kryo 360 Gold & 6x1.7 GHz Kryo 360 Silver)
GPU     | Adreno 616
Memory  | 4/6 GB RAM
Shipped Android Version | 8.1 with MIUI 9.5
Storage | 64/128 GB, non-expandable
Battery | Non-removable Li-Ion 3120 mAh battery, supports Quick Charge 3.0
Display | 	5.88 inches, 1080 x 2244 pixels, 18.7:9 ratio, Super AMOLED (~423 ppi density)
Camera  |Dual: 12 MP + 5 MP, f/1.9 aperture, Dual Pixel PDAF, dual-LED flash 20 MP, f/2.0 aperture

## Device picture

![Xiaomi Mi 8 SE](https://fdn2.gsmarena.com/vv/bigpic/xiaomi-mi8-se.jpg "Xiaomi Mi 8 SE in black")

## Building
Generally, see https://wiki.orangefox.tech/en/dev/building

This device tree inherits from the common sdm845 device tree (device/xiaomi/sdm845-common),
which is cloned automatically by vendorsetup.sh.

```
lunch twrp_sirius-eng

### Variants
1. For standard mode, build without any additional flags.
2. To build for ROMs using retrofitted dynamic partitions, run "export FOX_USE_DYNAMIC_PARTITIONS=1" before building.
3. To build for ROMs using borrowed keymaster 4.0, run "export FOX_USE_KEYMASTER_4=1" before building.
```

## Copyright
 ```
  /*
  *  Copyright (C) 2018 The LineageOS Project
  *
  *  Copyright (C) 2019-2026 The OrangeFox Recovery Project
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
  *
  * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU General Public License
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  *
  */
  ```
