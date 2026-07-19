<div align="center">

# Luoka

嵌入式开发学习者 · 热衷从裸机寄存器到上位机可视化的完整闭环

[![GitHub followers](https://img.shields.io/github/followers/Luoka666?style=social)](https://github.com/Luoka666)

</div>

---

### 技术栈

![C](https://img.shields.io/badge/C-主语言-5555ff?style=flat&logo=c)
![Python](https://img.shields.io/badge/Python-上位机开发-3776AB?style=flat&logo=python)
![STM32](https://img.shields.io/badge/STM32-F103C8T6-03234B?style=flat&logo=stmicroelectronics)
![FreeRTOS](https://img.shields.io/badge/FreeRTOS-学习中-8cc63f?style=flat)
![Keil](https://img.shields.io/badge/Keil-MDK-aaaaaa?style=flat&logo=arm)
![Git](https://img.shields.io/badge/Git-版本管理-F05032?style=flat&logo=git)

GPIO / EXTI / TIM / PWM / I2C / USART / SysTick / 单总线 · 有限状态机 (FSM) / 非阻塞事件驱动 / 模块化分层设计

---

### 精选项目

#### 智能温湿度监测与报警系统

[![STM32](https://img.shields.io/badge/STM32F103-标准库-blue?style=flat)](https://github.com/Luoka666/STM32F103_Loka_Project/tree/main/Temperature_Humidity_Sensor_Alarm_System)
[![配套上位机](https://img.shields.io/badge/配套-Python上位机-green?style=flat)](https://github.com/Luoka666/upper_computer)

> 从传感器驱动到 PC 端可视化，实现完整物联网数据闭环

- **双层状态机** — 7 种系统状态，按键 → 状态跳转 → 行为执行三层解耦
- **非阻塞报警** — SysTick 毫秒中断驱动，LED + 蜂鸣器报警不阻塞主循环
- **底层驱动** — 独立编写 DHT11 单总线、I2C OLED、USART 串口驱动
- **环形缓冲区** — 历史数据存储与 UI 显示解耦
- **防误触设计** — RUN 状态下主动锁定菜单键
- **软硬件联调** — 编写独立硬件测试用例定位并解决 GPIO 配置错误、电源轨断路等故障

[>> 项目文档（含完整踩坑记录）](https://github.com/Luoka666/STM32F103_Loka_Project/tree/main/Temperature_Humidity_Sensor_Alarm_System)

---

#### Python 串口上位机

[![Python](https://img.shields.io/badge/Python-3.8+-blue?style=flat)](https://github.com/Luoka666/upper_computer)

> 接收 STM32 下位机数据，PC 端实时双 Y 轴动态曲线显示

- **非阻塞串口读取** — `in_waiting` 轮询替代阻塞式 `readline()`，动画不卡顿
- **断线自动重连** — 状态机管理连接状态，2 秒重试间隔，程序不退出
- **智能视图管理** — 用户查看历史数据时自动暂停滚动，一键跳回最新
- **跨语言联调** — Python 上位机 × C 下位机，独立完成协议对齐与联调

[>> 项目文档](https://github.com/Luoka666/upper_computer)

---

### 学习路径

| 阶段 | 项目 | 技能点 |
|------|------|--------|
| 入门 | LED 闪烁、流水灯、蜂鸣器 | GPIO 输出控制 |
| 输入 | 按键控制、光敏传感器 | GPIO 输入、消抖、ADC |
| 显示 | OLED 驱动 | I2C 通信 |
| 中断 | 红外传感器、旋转编码器 | EXTI 外部中断 |
| 定时 | 定时器中断、PWM 呼吸灯、舵机 | TIM、PWM 占空比 |
| 综合 | **温湿度监测与报警系统** | FSM + 多外设协同 + 软硬件联调 |
| 集成 | **Python 上位机** | 串口协议 + 数据可视化 |

[>> 完整学习仓库（15 个项目）](https://github.com/Luoka666/STM32F103_Loka_Project)

---

### 其他项目

- [贪吃蛇](https://github.com/Luoka666/Hungry-Snake) — C 语言控制台游戏，含移动、食物生成、碰撞检测
- [FreeRTOS 学习](https://github.com/Luoka666/FreeRTOS_Learning) — 任务调度与队列通信实战

---

<div align="center">

**AI 辅助开发** — 熟练使用 Claude Code、GitHub Copilot、ChatGPT 辅助编码、Review、调试与文档编写

</div>