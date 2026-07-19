<div align="center">

# 李佳乐 | Luoka

### 嵌入式软件开发实习生

[![Email](https://img.shields.io/badge/邮箱-3266380141@qq.com-blue?style=flat&logo=gmail)](mailto:3266380141@qq.com)
[![Phone](https://img.shields.io/badge/电话-18706805618-green?style=flat&logo=whatsapp)](tel:18706805618)
[![GitHub](https://img.shields.io/badge/GitHub-Luoka666-black?style=flat&logo=github)](https://github.com/Luoka666)

</div>

---

### 教育背景

**西安建筑科技大学华清学院** · 计算机科学与技术（本科） · 2023.09 ~ 2027.06

---

### 技术能力

| 分类 | 技能 |
|------|------|
| **编程语言** | C（指针、结构体、位运算）、Python（串口上位机开发） |
| **MCU 平台** | STM32F103C8T6，标准外设库（StdPeriph） |
| **外设与协议** | GPIO、USART、I2C、PWM、SysTick、单总线（DHT11） |
| **嵌入式技能** | 有限状态机（FSM）、非阻塞任务调度、模块化分层设计 |
| **开发工具** | Keil MDK、CLion、Git、串口调试助手 |
| **AI 辅助开发** | Claude Code、GitHub Copilot、ChatGPT — 辅助编码、Review、调试、文档 |

---

### 项目经验

#### 智能温湿度监测与报警系统 [>> 项目链接](https://github.com/Luoka666/STM32F103_Loka_Project/tree/main/Temperature_Humidity_Sensor_Alarm_System)
STM32F103 + DHT11 + OLED + 蜂鸣器 | 独立开发 | 2026.04 ~ 至今

- 设计 **7 种系统状态**的双层 switch-case 状态机，实现按键、逻辑、UI 三层解耦
- 独立编写 DHT11 单总线、I2C OLED、USART 串口等底层驱动
- 基于 SysTick 毫秒中断实现 LED + 蜂鸣器**非阻塞报警**，消除传统 Delay 阻塞风险
- 实现**环形缓冲区**存储历史数据，解决数据与显示耦合问题
- 状态切换统一清屏机制解决 OLED 字符残留；RUN 状态下锁定菜单键防止误触
- 编写独立硬件测试用例定位 GPIO 配置错误、电源轨断路等软硬件联合故障

#### Python 串口数据可视化上位机 [>> 项目链接](https://github.com/Luoka666/upper_computer)
Python + PySerial + Matplotlib | 独立开发 | 2026.06 ~ 至今

- 自定义 ASCII 文本协议，正则解析 STM32 串口数据，支持**断线自动重连**
- Matplotlib 双 Y 轴动态曲线，100ms 刷新率，全量存储支持历史回溯
- 智能视图管理：检测用户操作自动切换跟随滚动/固定视图模式
- 独立完成 Python 上位机与 C 下位机的**跨语言联合调试**

#### 其他项目
| 项目 | 说明 |
|------|------|
| [STM32 学习之路](https://github.com/Luoka666/STM32F103_Loka_Project) | 15 个实战项目，从 GPIO 到 PWM，覆盖 STM32 主要外设 |
| [贪吃蛇](https://github.com/Luoka666/Hungry-Snake) | C 语言控制台游戏，含蛇身移动、食物生成、碰撞检测 |
| [FreeRTOS 学习](https://github.com/Luoka666/FreeRTOS_Learning) | FreeRTOS 任务调度、队列通信入门实战 |

---

### 自我评价

具备独立完成嵌入式项目从驱动开发到系统集成的全流程能力。习惯在开发中借助 AI 工具提升效率，同时坚持理解每一行代码的原理。善于通过调试定位软硬件联合故障并记录踩坑经验，具备良好的工程文档习惯。

---

<div align="center">

**正在寻找嵌入式软件实习机会，欢迎联系**

</div>