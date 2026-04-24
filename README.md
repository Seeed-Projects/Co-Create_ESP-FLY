# ESP-FLY DIY Kit

![ESP-FLY Overview](https://files.seeedstudio.com/products/114993694/img/1-114993694-ESP-FLY-DIY-Kit.jpg)

## Short Description

The ESP-FLY is a compact, lightweight DIY micro drone kit powered by the Seeed Studio XIAO ESP32-S3. This product is a Co-Create collaboration with Seeed Studio and **Max Imagination**. Designed for STEM education and hobbyists, it offers dual control methods via Wi-Fi (mobile app) or ESP-NOW (radio controller), providing a fun, hands-on way to understand electronics and aerial robotics.

The XIAO ESP32S3 acts as the main flight controller and communicates with a custom motor driver / IMU board to control four high-speed coreless motors. The result is a lightweight 50 mm class micro drone that can be assembled, programmed, and flown for experimentation, education, and hobby use.

## Features

- **Two control methods**
  - Fly from your phone using the drone's 2.4 GHz Wi-Fi Access Point with the ESP-Drone mobile app.
  - Or use a radio controller via an ESP-NOW TX link for better control precision and longer range.

- **ESP32-S3 flight controller**
  - Based on the Seeed Studio XIAO ESP32S3.
  - Dual-core 240 MHz Xtensa LX7 CPU with 2.4 GHz Wi-Fi and Bluetooth support.

- **Custom 4-layer flight controller PCB**
  - Integrates the MPU-6050 6-axis IMU (gyro + accelerometer).
  - Includes four N-channel MOSFET motor drivers.
  - Includes onboard LEDs for status and orientation indication.

- **Lightweight airframe**
  - 3D-printed 50 mm frame with a compact closed-body design.
  - Frame weight is approximately 4 g.

- **High thrust-to-weight ratio**
  - Four 6 × 15 mm coreless motors.
  - Combined thrust is sufficient for stable indoor flight and light outdoor use in calm conditions.

- **Optional FPV support**
  - Frame includes an optional top cover for a micro FPV camera.
  - Compatible with lightweight 5.8 GHz AIO analog FPV camera modules.

- **Open-source firmware options**
  - Supports Espressif's ESP-Drone firmware.
  - Also supports rtlopez's ESP-FC firmware for Betaflight-compatible workflows.

- **USB-C programming and charging**
  - The XIAO ESP32S3 USB-C port can be used for firmware upload and LiPo charging.

## Description

ESP-FLY is a compact DIY ESP32 quadcopter kit intended for learning and experimentation. Powered by the Seeed Studio XIAO ESP32S3 and stabilized with a 6-axis IMU, it provides a practical platform for exploring micro drone assembly, embedded control, and wireless flight.

The drone can be operated in two main ways:

1. **Wi-Fi control with ESP-Drone**
   - The drone creates its own local Wi-Fi AP.
   - A phone can connect directly to it without requiring a router.
   - This provides a simple way to fly and test the platform with low-latency input.

2. **Radio control with ESP-FC**
   - With rtlopez's ESP-FC firmware, the drone can be paired with a radio controller over ESP-NOW.
   - This enables more advanced control workflows and configuration through Betaflight.

The hardware consists of a custom lightweight flight controller PCB with integrated IMU, motor drive stage, and onboard LEDs, with the XIAO ESP32S3 stacked on top as the main controller. The airframe uses a compact 3D-printed structure, and the top cover can be swapped for an FPV version when first-person-view flying is desired.

With the included 1S 250 mAh LiPo battery, the platform has been tested for up to about 5.5 minutes of flight time under suitable conditions. The design also includes failsafes to reduce the chance of flyaways in case of signal loss.

## Project Resources

- **ESP-FLY Drone Tutorial Video** https://www.youtube.com/watch?v=V_mZsiZcy7s

- **ESP-FLY Tutorial Blog** https://www.elektormagazine.com/labs/esp-fly-the-smallest-esp32-drone-you-can-build

- **Radio Controller + Betaflight Firmware Tutorial** https://www.youtube.com/watch?v=QTmitUFotik

## Application

- STEM education and classroom learning
- DIY maker projects
- Indoor FPV flying and training
- Research and prototyping
- Hobby experimentation and fun

## Specifications

| Item | Specification |
|---|---|
| Microcontroller | Seeed Studio XIAO ESP32S3 |
| Processor | Dual-core 240 MHz Xtensa LX7 |
| Memory | 8 MB Flash, 8 MB PSRAM |
| Wireless | Wi-Fi, Bluetooth 5.0 |
| IMU Sensor | MPU-6050 6-DoF |
| Motor Drivers | 4 × SI2300 N-channel MOSFETs |
| Motors | 4 × 615 coreless DC motors (70,000 RPM, approx. 17 g thrust each) |
| Dimensions | 67 × 67 × 31 mm (including propellers) or 46 × 46 × 29 mm (excluding propellers) |
| Frame Class | 50 mm micro drone |
| Weight | ~18 g / 25 g / 28 g (without LiPo / with LiPo / with FPV camera) |
| Battery | 1S Li-Po 3.7 V, 250 mAh, JST-PH 2-pin |
| Flight Time | Estimated ~5 minutes typical, up to ~5.5 minutes tested |
| Control Method | Wi-Fi via smartphone app (ESP-Drone) / ESP-NOW via radio controller |
| Control Range | Approx. 50 m via Wi-Fi / up to approx. 200 m via ESP-NOW |
| Flight Modes | Angle and Acro |
| FPV Support | Optional micro FPV camera support |
| Programming Interface | USB-C |
| Development Tools | ESP-IDF / VS Code + PlatformIO / Betaflight Configurator |

## Hardware Overview

ESP-FLY is built around two main hardware blocks:

- **Seeed Studio XIAO ESP32S3**
  - Main MCU
  - Wireless communication
  - Flight control logic
  - USB-C interface for programming and charging

- **Custom IMU / Motor Driver Module**
  - MPU-6050 for motion sensing
  - MOSFET motor drivers for four brushed motors
  - Power routing and LED indicators

The drone frame supports both a standard top cover and an optional FPV top cover.

![ESP-FLY Hardware Overview](https://files.seeedstudio.com/products/114993694/img/ESP-FLY_hd1.jpg)
![ESP-FLY Hardware Overview](https://files.seeedstudio.com/products/114993694/img/ESP-FLY_hd2.jpg)

## Parts List (Included in the Kit)

- 1 × Seeed Studio XIAO ESP32-S3 microcontroller with pre-soldered headers
- 1 × 2.4G Antenna for XIAO ESP32-S3
- 1 × IMU / motor driver module (pre-assembled)
- 2 × 24AWG red/black wires for joining battery power to the XIAO
- 4 × coreless motors (6 × 15 mm), including 2 CW and 2 CCW motors with pre-attached wires
- 8 × propellers (30 mm tri-blade), including 4 CW and 4 CCW props
- 1 × 1S LiPo battery (3.7 V, 250 mAh)
- 1 × 3D-printed parts set: frame, standard top cover, and optional FPV top cover
- 1 × "ESP-FLY" sticker
- 1 × battery-mounting zip-tie
- 4 × landing gear enameled solid wires

## Not Included

- Soldering iron and solder
- Tweezers / helping hands / flush cutters / hobby knife
- Prop remover tool
- Superglue
- Smartphone or radio controller
- FPV equipment (camera / VTX module / goggles / monitor)
- USB-C cable
- Computer for firmware upload or modification

## Open Source License & Declaration

The firmware provided in this repository is a modified version based on the original ESP-Drone project by Espressif and the modified version by Circuit Digest. In accordance with the GPL-3.0 License, this software is provided "AS IS", without warranty of any kind.

Please note: Seeed Studio and the creator (Max Imagination) are primarily responsible for the hardware design and structural integrity of the ESP-FLY kit.

## FAQ

### 1. What is the flight time and control range?

Typical flight time is about **5 minutes**, with **up to 5.5 minutes** tested under suitable conditions.  
Control range is approximately **50 meters line of sight** over Wi-Fi, and can be extended when using an ESP-NOW radio controller setup.

### 2. Can I use a different battery size or add payload?

Yes. A **150–350 mAh** battery with an appropriate discharge rate can be used, but larger batteries will add weight and may reduce agility and flight time.  
With the included 250 mAh battery, the recommended maximum payload is about **3 g**.

### 3. Can I add an ESP32 camera for FPV?

Not directly with the current open-source firmware workflow on the XIAO.  
However, the frame supports a lightweight **5.8 GHz analog AIO FPV camera** for first-person-view flying.

### 4. Does ESP-FLY support altitude hold, GPS, or autonomous flight?

No. ESP-FLY is a manually controlled micro drone platform.  
It supports self-leveling in **Angle mode**, but does not include altitude hold, GPS, or autonomous navigation features.

### 5. How difficult is the assembly?

Assembly is relatively straightforward and mainly requires **basic soldering**:
- connect the XIAO to the IMU / motor driver board
- solder the motor wires
- assemble the frame and drivetrain

This makes ESP-FLY suitable for beginners who want a small but practical drone hardware project.