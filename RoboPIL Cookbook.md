# 🔮 RoboPIL Cookbook 🧑‍🍳

> **Contributors** (no sequence):
>
> Guang Yin (guangy2@illinois.edu)
>
> Binghao Huang (binghao2@illinois.edu)

## Preface

Nice to meet you, and welcome to RoboPIL! I am a cookbook you should read before eagerly playing with equipment without considering any **safety** issues. Also, technically, I am a complete reference hardware manual, so if you have any questions about anything in the lab, you should revisit me first. If new equipment arrives or you get the answer that others may be concerned about, please feed me 😋 **NOW!**

## Table of Contents

[TOC]

## xArm 🦾

### Online Resources

- [Product Downloads](https://www.ufactory.cc/download)
- [User Manual](https://www.ufactory.cc/wp-content/uploads/2023/05/xArm-User-Manual-V2.0.0.pdf)
- [Developer Manual](https://www.ufactory.cc/wp-content/uploads/2023/04/xArm-Developer-Manual-V1.10.0.pdf)
- [3D Files](https://www.ufactory.cc/wp-content/uploads/2023/04/xArm6XI1300.zip)

### Software and Python SDK

- [UFACTORY Studio](https://www.ufactory.cc/ufactory-studio)

  This is the software used to manually control the xArm or reset its position.

  ![image-20231205173413235](./RoboPIL%20Cookbook.assets/image-20231205173413235.png)

  > Remember to set the AppImage program as executable if you can’t open it.

- [xArm-Python-SDK](https://github.com/xArm-Developer/xArm-Python-SDK)

  This codebase includes Python API that you will integrate into your project to control the xArm.

  Download and install:

  ```sh
  git clone https://github.com/xArm-Developer/xArm-Python-SDK.git
  cd xArm-Python-SDK
  python setup.py install
  ```
  
  Integrate the SDK into your project:
  
  ```python
  from xarm.wrapper import XArmAPI
  ```

### Before Using

1. Check Ethernet connection and power supply

   ![image-20231205170338374](./RoboPIL%20Cookbook.assets/image-20231205170338374.png)

2. Change your wired connection IPv4 address to `192.168.1.*`

   > whatever for the last address block

   ![image-20231205173018759](./RoboPIL%20Cookbook.assets/image-20231205173018759.png)

3. Turn on the OFF/ON switch and ensure the indicator lights are lit

   ![image-20231205171331103](./RoboPIL%20Cookbook.assets/image-20231205171331103.png)

4. Release the emergency stop

   ![image-20231205171712003](./RoboPIL%20Cookbook.assets/image-20231205171712003.png)

5. Open UFACTORY Studio and enter the IP address of the control box `192.168.1.209`

   ![image-20231205172720941](./RoboPIL%20Cookbook.assets/image-20231205172720941.png)

6. Press `Enable Robot` and have FUN!

   ![image-20231205172751325](./RoboPIL%20Cookbook.assets/image-20231205172751325.png)

### After Using

1. Push down the emergency button

2. Press the black PWR button for 5 seconds until indicator lights are off

   ![image-20231205174852114](./RoboPIL%20Cookbook.assets/image-20231205174852114.png)

3. Turn off the OFF/ON switch

### Direct-drive Linear Motor

To Be Continued… 🚧

### Gripper

To Be Continued… 🚧

### Vacuum Gripper

To Be Continued… 🚧

### 6 Axis Force Torque Sensor

To Be Continued… 🚧

## ALOHA 🏖️

### Online Resources

- [Official Website](https://tonyzhaozh.github.io/aloha)

To Be Continued… 🚧

## GELLO 🕹️

### Online Resources

- [Official Website](https://wuphilipp.github.io/gello_site)
- [Official repo for software](https://github.com/wuphilipp/gello_software)
- [Official repo for hardware](https://github.com/wuphilipp/gello_mechanical)
- [Guang’s modified version for xArm6](https://github.com/AlchemicRonin/GELLO)

### Preparation

Download the repo

```sh
git clone https://github.com/AlchemicRonin/GELLO.git
cd GELLO
```

Create your environment

```sh
git submodule init
git submodule update
pip install -r requirements.txt
pip install -e .
pip install -e third_party/DynamixelSDK/python
```

### Running on xArm6

In one terminal, run the following command:

```
python experiments/launch_nodes.py --robot=xarm
```

Open another terminal, and run:

```
python experiments/run_env.py --agent=gello
```

To Be Continued… 🚧

## STAG 🤙

### Online Resources

- [Official Website](http://stag.csail.mit.edu)

To Be Continued… 🚧

## RealSense 📷

### Online Resources

- [Official Website](https://www.intelrealsense.com/depth-camera-d455)

### Calibration

To Be Continued… 🚧

### Point Cloud

To Be Continued… 🚧

## SSH 📟

To Be Continued… 🚧

## NeoVim 🛸

![image-20231205175719589](./RoboPIL%20Cookbook.assets/image-20231205175719589.png)

To Be Continued… 🚧