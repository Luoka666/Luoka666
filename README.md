# Luoka · 嵌入式软件开发

您好，我是李佳乐，2027 届计算机科学与技术本科生，求职方向为嵌入式软件开发实习。

目前主要使用 **C、STM32F103 和 FreeRTOS**，通过项目练习外设驱动、状态机、多任务通信与软硬件联调，并使用 Python 开发配套串口工具。

## 先看这两个项目

| 项目 | 实现内容 | 推荐阅读入口 |
| --- | --- | --- |
| **STM32 温湿度监测与报警系统** | DHT11 采集、OLED 菜单、阈值报警、历史记录；裸机与 FreeRTOS 双版本 | [项目总览](https://github.com/Luoka666/STM32F103_Loka_Project) · [裸机版](https://github.com/Luoka666/STM32F103_Loka_Project/tree/main/Temperature_Humidity_Sensor_Alarm_System_BareMetal) · [FreeRTOS 版](https://github.com/Luoka666/STM32F103_Loka_Project/tree/main/Temperature_Humidity_Sensor_Alarm_System_FreeRTOS) |
| **Python 串口可视化上位机** | 接收下位机数据，绘制温湿度双 Y 轴曲线，支持历史浏览和断线重连 | [使用方法与源码](https://github.com/Luoka666/upper_computer) |

### 温湿度系统里重点做了什么

- **裸机调度**：7 状态有限状态机，按键扫描、传感器采样与报警各自计时；非阻塞消抖避免长按占用主循环。
- **多任务协作**：6 个 FreeRTOS 任务、4 条消息队列；使用互斥量保护 OLED 与历史记录访问。
- **异常处理**：DHT11 电平等待增加超时；显示和报警队列覆盖旧值，历史队列满时淘汰最旧待处理数据，避免采集任务长期阻塞。
- **联调记录**：记录 GPIO 时钟及端口配置、面包板电源轨、SysTick 延时冲突等问题的定位过程。

下位机通过串口发送采样结果，上位机解析并显示，构成一套可以联合调试的监测系统。

## 技术实践

| 方向 | 项目中使用的技术 |
| --- | --- |
| MCU 与外设 | STM32F103C8T6、标准外设库、GPIO、USART、TIM、SysTick、软件 I2C、DHT11 单总线 |
| 系统组织 | 有限状态机、非阻塞按键消抖、环形缓冲区、FreeRTOS 任务、队列、互斥量 |
| PC 工具 | Python、PySerial、Matplotlib、串口数据解析 |
| 开发与调试 | Keil MDK、CLion、Git、串口日志、独立硬件测试程序 |

## 学习与练习仓库

- [STM32 外设练习](https://github.com/Luoka666/STM32F103_Loka_Project#外设练习索引)：GPIO、中断、定时器、PWM 和 OLED 等基础练习，与综合项目分开列出。
- [FreeRTOS 学习](https://github.com/Luoka666/FreeRTOS_Learning)：实时操作系统的学习与实验记录。
- [数据结构与算法](https://github.com/Luoka666/Data-Structures-and-Algorithms)：C 语言实现，使用 CMake 管理，按数据结构和算法分类整理。
- [C 语言贪吃蛇](https://github.com/Luoka666/Hungry-Snake)：控制台游戏练习。

## 联系方式

邮箱：[3266380141@qq.com](mailto:3266380141@qq.com)
