# MAX30102血氧传感器数据采集与OLED显示代码

## 项目描述

本项目提供了一个基于STM32F103C8T6芯片的MAX30102血氧传感器数据采集与OLED显示的代码。该代码实现了通过STM32F103C8T6芯片与MAX30102传感器进行通信，采集血氧和脉搏数据，并通过0.96寸OLED显示屏实时显示数据。同时，数据还可以通过串口传输到PC端。

## 硬件连接

### MAX30102传感器与STM32F103C8T6的接口

- SDA -------- PB9
- SCL -------- PB8
- INT -------- PB7
- VCC -------- 3.3V
- GND -------- GND

### OLED显示屏与STM32F103C8T6的接口

- GND -------- GND
- VDD -------- 3.3V
- SCK -------- E0
- SDA -------- G15

## 功能说明

1. **数据采集**：通过MAX30102传感器采集血氧和脉搏数据。
2. **数据处理**：对采集到的数据进行平均处理，取10次有效值的平均值。
3. **OLED显示**：在0.96寸OLED显示屏上显示“血氧/脉搏：血氧数值/脉搏数值”。
4. **串口传输**：通过MINIUSB线将数据通过串口传输到PC端。

## 使用说明

1. **初始化**：在开始测量前，系统会显示“Invalid”状态，等待10秒钟后，系统会自动开始测量并显示数据。
2. **数据传输**：通过MINIUSB线连接STM32F103C8T6与PC，可以直接进行串口数据传输，无需额外的USB转TTL模块。

## 注意事项

- 在测试过程中，请确保传感器与STM32F103C8T6的连接正确，避免信号干扰。
- 数据采集和显示过程中，请保持传感器与手指的稳定接触，以确保数据的准确性。

## 贡献

欢迎大家提出改进建议或提交代码优化，共同完善本项目。

## 下载链接
[MAX30102血氧传感器数据采集与OLED显示代码](https://pan.quark.cn/s/639c7bec5c0d) 

(备用: [备用下载](https://pan.baidu.com/s/19zicIrdS58pFKxqGdpyMhw?pwd=tqqh))

## 说明

该仓库仅用于学习交流，请勿用于商业用途。
