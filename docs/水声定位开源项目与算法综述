# 水声定位开源项目与算法综述

> **日期**: 2026-08-18
> **范围**: 水下声学定位（LBL / SBL / USBL / TDOA / 深度学习）
> **项目数**: 12+ | **算法**: 9 类

---

## 一、概述

水声定位（Underwater Acoustic Positioning）是利用声波在水中的传播特性，通过测量信号的传播时间、相位差或到达角度等参数来实现水下目标定位的技术。由于无线电波在水下衰减极快，声波成为水下远程通信和定位的首选介质 [1]。

### 定位方式分类

根据基线长度（参考点之间的距离），水声定位主要分为三类：

| 方式 | 全称 | 基线长度 | 精度 | 适用范围 |
|------|------|----------|------|----------|
| **LBL** | Long Baseline 长基线 | 100m ~ 数 km | 厘米~分米级 | 大范围 |
| **SBL** | Short Baseline 短基线 | 1m ~ 50m | 分米~米级 | 中等范围 |
| **USBL** | Ultra-Short Baseline 超短基线 | < 1m | 米级 | 中小范围 |

此外，还有**虚拟长基线（VLBL）**、**基于深度学习的水声定位**等新兴方向。近年来，随着水下机器人（ROV/AUV）的普及，开源社区涌现了多个水声定位相关项目 [2][3]。

---

## 二、开源项目总览

| 项目名称 | 定位方式 | 语言 | 许可证 | 特点 | 活跃度 |
|----------|----------|------|--------|------|--------|
| **Raspi²USBL** | USBL (倒置) | C++ | 开源 | 树莓派硬件方案，实时信号处理 | 活跃 (2025) |
| **UCNLNav** | TDOA / TOA / AOA / VLBL | C# / Rust / Matlab | GPL-3.0 | 导航算法库，多语言实现 | 活跃 (2026) |
| **WAYU** | LBL | C# | 开源 | 完整 LBL 跟踪系统，含硬件设计 | 维护中 |
| **USBL-Simulator** | USBL (仿真) | C++ / ROS 2 | MIT | ROS2 仿真器，含噪声建模 | 活跃 (2025) |
| **EviNS Framework** | LBL / USBL / SBL / 协同定位 | C++ / Python | 开源 | EvoLogics 调制解调器框架，ROS 集成 | 活跃 |
| **UnetStack** | OWTT / LBL / USBL | Java / Julia / Groovy | 社区版免费 | 完整仿真+部署平台，含 USBL 算法 | 活跃 |
| **UnderwaterAcousticTracker** | TDOA / TOA | Python | 开源 | SIO 实验室，VOLT 定位 | 低活跃 |
| **acoustic-location-system** | 声学定位 | Python | 开源 | 面向小型 ROV (OpenROV)，含硬件设计 | 低活跃 |
| **UWSL-APP** | 水声源定位 (深度学习) | Python / Matlab | 开源 | 神经网络定位，多深度数据集 | 活跃 (2025) |
| **Echoscope** | 主动声纳回波定位 | JavaScript | 开源 | 浏览器端运行，匹配滤波/波束成形 | 活跃 |
| **WHOI Micro-Modem 生态** | LBL / OWTT | C++ (MOOS) | 部分开源 | MIT 标准生态，MOOS-IvP 集成 | 维护中 |
| **beamforming-tools** | 波束成形 / DOA | 多语言 | 开源 | 波束成形工具索引，含声学成像 | 活跃 (2026) |

---

## 三、核心项目详解

### 3.1 Raspi²USBL

- **仓库**: https://github.com/ethanjinhuang/Raspi2USBL
- **语言**: C++
- **定位方式**: USBL（倒置）/ OWTT
- **最近提交**: 2026-07 | 提交数: 5 | 论文: arXiv:2511.06998

2025 年发布的**开源树莓派倒置 USBL 定位系统**，是目前最完整的开源 USBL 硬件+软件方案 [4]。该系统基于 Raspberry Pi 平台，采用被动式倒置超短基线架构，可实现高精度时钟同步和单向传播时间（OWTT）消息通信。

**核心特性**:
- **信号处理**: 实时匹配滤波、阵列波束成形、自适应增益控制
- **核心功能**: 飞行时间（TOF）估计、到达方向（DOA）估计
- **验证场景**: 消声水池、淡水湖泊、海上试验均已完成验证
- **原始数据**: 仓库附带原始采集数据和 Matlab 处理代码，便于研究者快速分析

---

### 3.2 UCNLNav

- **仓库**: https://github.com/ucnl/UCNLNav
- **语言**: C# / Rust / Matlab
- **定位方式**: TDOA / TOA / AOA / VLBL
- **许可证**: GPL-3.0
- **最近提交**: 2026-07 | 提交数: 145 | 持续更新中

由 ucnl 团队维护的**多语言导航算法库**，覆盖了水声定位中绝大多数核心定位算法 [5]。提供 C#、Rust、Matlab 三种语言实现，是算法学习和快速原型开发的理想选择。

**核心特性**:
- **TDOA / TOA**: 2D 和 3D 时空差定位求解
- **AOA**: 到达角度导航问题求解
- **VLBL**: 虚拟长基线定位算法
- **大地测量**: Haversine / Vincenty 公式、UTM 坐标转换
- **优化算法**: Nelder-Mead、Hooke-Jeeves 等无梯度优化
- **精度评估**: DOP 计算、CEP/SEP/DRMS 统计

---

### 3.3 WAYU (Where Are You Underwater)

- **仓库**: https://github.com/ucnl/WAYU
- **语言**: C#
- **定位方式**: LBL
- **最近发布**: 2021 | 语言: C# 100%

同样来自 ucnl 团队的 **LBL 长基线水声定位系统**，是 WAYU Pinger 硬件配套的软件端 [5]。可追踪搭载 WAYU Pinger 的潜水员、ROV、AUV 等水下目标。

**核心特性**:
- 完整的 LBL 定位系统应用，含水面端软件
- 基于 UCNLNav 算法库构建
- 支持地理坐标输出（经纬度）
- 适合 DIY 水声定位项目参考

---

### 3.4 USBL-Simulator

- **仓库**: https://github.com/maximilian-nitsch/USBL-Simulator
- **语言**: C++ / ROS 2
- **定位方式**: USBL 仿真
- **许可证**: MIT
- **最近提交**: 2025-04 | 提交数: 16

基于 **C++/ROS 2 的超短基线（USBL）仿真器**，专为水下机器人导航算法开发和测试设计 [6]。提供完整的 USBL 测量仿真链路，支持噪声和量化建模。

**核心特性**:
- **USBL 阵列仿真**: 换能器和水听器位置建模
- **双模式**: 标准 USBL 配置和倒置 USBL 配置（USBL 在水面、应答器在 AUV 上）
- **噪声建模**: 往返时间（RTT）噪声与量化、TDOA 噪声与量化
- **IMU 仿真**: 内置 AHRS（姿态航向参考系统）仿真
- 从 TRIPLE GitLab 迁移至 GitHub，有 CI/CD 流水线

---

### 3.5 EviNS Framework

- **仓库**: https://github.com/EvoLogics/evins
- **语言**: C++ / Python
- **定位方式**: LBL / USBL / SBL / 协同定位
- **许可证**: 开源
- **维护方**: EvoLogics 公司

由 EvoLogics 公司开发的**水下声学传感器网络与定位系统开发框架** [7]。采用事件驱动编程范式，可直接运行于 EvoLogics 声学调制解调器上，支持从开发、测试到部署的全流程。

**核心特性**:
- **多定位方式**: LBL、USBL/SBL、协同定位
- **ROS 集成**: 提供 evins_nl（ROS 驱动）和 evins_ros_docker（Docker 部署）
- **开放架构**: 支持第三方声学调制解调器接入
- **DMACE 工具集**: 开发、测试、部署、运维全链路工具
- 已在多个海洋物联网项目中实际应用

---

### 3.6 UnetStack

- **官网**: https://unetstack.net
- **语言**: Java / Julia / Groovy
- **定位方式**: OWTT / LBL / USBL
- **许可证**: 社区版免费（教育研究用）
- **维护方**: ARL（新加坡国立大学水下研究实验室）

**水下网络协议栈与仿真平台**，社区版免费用于教育和研究 [8]。提供从算法仿真到实际部署的完整工作流，是目前最成熟的水声网络开发平台之一。

**核心特性**:
- **Unet Simulator**: 离散事件仿真，支持蒙特卡洛测试
- **USBL 实现**: unet-contrib 仓库含 usbl-julia 模块，可将多接收器调制解调器变为 USBL 收发器 [9]
- **定位示例**: 官方博客有基于 OWTT 的水下定位完整教程
- **Unet IDE**: 集成开发环境，支持代理和协议开发
- 支持从仿真直接迁移到真实调制解调器部署

---

### 3.7 UWSL-APP（水下声源定位）

- **仓库**: https://github.com/Perry44001/UWSL-APP
- **语言**: Python / Matlab
- **定位方式**: 深度学习
- **最近更新**: 2025-03

**基于神经网络的水下声源定位应用**，采用 Matlab App 生成数据集 + Python 训练定位模型的混合架构 [10]。代表了水声定位的深度学习新方向。

**核心特性**:
- 支持不同海深的数据集训练和测试
- 输出距离和深度的联合定位结果
- 模型训练参数可视化（阵元数、频点数、批次大小、学习率等）
- 提供训练误差和测试精度的量化对比

---

### 3.8 其他值得关注的项目

#### UnderwaterAcousticTracker
- **仓库**: https://github.com/SIOJaffeLab/UnderwaterAcousticTracker
- SIO Jaffe Lab 开发的声学追踪代码，使用 TDOA/TOA 算法对 VOLT（水下声学追踪器）进行定位。

#### acoustic-location-system
- **仓库**: https://github.com/Jlsmith10/acoustic-location-system
- 面向小型水下 ROV（如 OpenROV）的声学定位系统，包含软件和硬件设计。有 DSP 测试数据分析功能。

#### Echoscope
- **仓库**: https://github.com/lifeart/echoscope
- 浏览器端运行的主动声纳回声定位系统，利用设备扬声器发射声学探测信号，通过麦克风回波和匹配滤波互相关来估计目标距离和方向。支持 Chirp、MLS、Golay、FDM/OFDM 等多种信号类型。

#### WHOI Micro-Modem 生态
- Woods Hole 海洋研究所的微型声学调制解调器，支持窄带和宽带 LBL 导航、调制解调器间测距和同步单向测距（OWTT）[11]。通过 MOOS-IvP 中间件（iWhoiMicroModem、pAcommsHandler）集成，是学术界水下声学通信的事实标准之一。硬件本身非开源，但软件接口和驱动开源。

#### beamforming-tools
- **仓库**: https://github.com/eac-ufsm/beamforming-tools
- 一个精心策划的**波束成形工具集合**，涵盖声学波束成形、到达方向估计、麦克风阵列处理、声学成像、机器人听觉、地震阵列分析和超声成像等方向。定期审查更新（最近审查：2026 年 7 月）。

---

## 四、核心算法汇总

水声定位涉及的核心算法可归纳为以下几类，它们在上述开源项目中各有体现：

| 算法 | 英文全称 | 说明 | 代表项目 |
|------|----------|------|----------|
| **TDOA** | Time Difference of Arrival | 通过多个接收器接收同一信号的时间差来定位目标。LBL/SBL 定位的基础算法 | UCNLNav, UnderwaterAcousticTracker |
| **TOA / OWTT** | Time of Arrival / One-Way Travel-Time | 直接测量信号传播时间计算距离。OWTT 为单向传播时间，需高精度时钟同步 | Raspi²USBL, UnetStack |
| **DOA / AOA** | Direction of Arrival / Angle of Arrival | 通过阵列信号处理估计信号到达方向，USBL 定位的核心 | Raspi²USBL, UCNLNav |
| **匹配滤波** | Matched Filtering / Cross-Correlation | 在已知信号波形下，通过互相关运算从噪声中提取信号到达时间 | Echoscope, Raspi²USBL |
| **GCC-PHAT** | Generalized Cross-Correlation with Phase Transform | 带相位变换的广义互相关算法，对混响环境鲁棒性好 | TDOA-Based DOA System |
| **阵列波束成形** | Array Beamforming | 通过对阵列各通道信号进行相位加权求和，增强特定方向的信号 | Raspi²USBL, Echoscope |
| **改进牛顿法** | Modified Newton Algorithm | 引入奇异值因子解决传统牛顿法不收敛问题，用于三维 USBL 定位 [12] | 学术算法 |
| **GAS 紧耦合滤波** | Globally Asymptotically Stable Filter | LBL/USBL 组合导航滤波器，不依赖代数反演和线性化，实现全局渐近稳定 [13] | 学术算法 |
| **VLBL** | Virtual Long Baseline | 利用运动平台在不同位置接收的信号，虚拟构造长基线阵列进行定位 | UCNLNav |
| **神经网络定位** | Neural Network Localization | 利用 CNN 等深度学习模型直接从声学信号估计目标位置 | UWSL-APP |

### 算法与项目覆盖矩阵

| 算法 \ 项目 | UCNLNav | Raspi²USBL | USBL-Sim | EviNS | UnetStack | UWSL-APP | Echoscope | WHOI MM |
|-------------|---------|------------|----------|-------|-----------|----------|-----------|---------|
| TDOA | ● | | ○ | ● | ○ | ○ | | ● |
| TOA/OWTT | ● | ● | ○ | ● | ● | | | ● |
| DOA/AOA | ● | ● | | ○ | | | ○ | |
| 匹配滤波 | | ● | | | | | ● | |
| 波束成形 | | ● | ○ | | | | | |
| VLBL | ● | | | | ○ | | | |
| 神经网络 | ○ | | | | | ● | | |
| GAS 滤波 | | | | | | | | |

> `●` = 完整实现 | `○` = 部分支持 | 空 = 未覆盖

---

## 五、技术生态全景

下图展示了从信号采集到定位输出的完整技术链路，以及各开源项目在其中的位置：

```
┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐
│    硬件层        │     │   信号处理层    │     │   定位算法层     │     │  仿真与部署层    │     │   导航融合层     │
├─────────────────┤     ├─────────────────┤     ├─────────────────┤     ├─────────────────┤     ├─────────────────┤
│ EvoLogics Modem │────▶│  匹配滤波       │────▶│  TDOA / TOA     │────▶│                 │────▶│  GAS 滤波器     │
│ Raspberry Pi    │────▶│  波束成形       │────▶│  DOA / AOA      │     │  UnetStack      │     │  卡尔曼滤波     │
│ WHOI Micro-Modem│────▶│  自适应增益控制  │     │  VLBL           │     │  USBL-Simulator │     │  SLAM           │
│ OpenROV 声学模块│     │                 │     │  神经网络       │     │  EviNS Framework│     │                 │
└─────────────────┘     └─────────────────┘     └─────────────────┘     └─────────────────┘     └─────────────────┘
```

---

## 六、选型建议

| 使用场景 | 推荐项目 | 理由 |
|----------|----------|------|
| **快速原型 / 算法学习** | UCNLNav | 多语言实现覆盖 TDOA/TOA/AOA/VLBL 全部核心算法，自带 Matlab 演示脚本，无需硬件即可上手 |
| **USBL 系统开发** | Raspi²USBL + USBL-Simulator | Raspi²USBL（2025 年最新，含完整 C++ 框架和实测数据）+ USBL-Simulator（ROS2 仿真环境），两者互补可覆盖从仿真到实测的全链路 |
| **完整网络仿真与部署** | UnetStack | 社区版免费，支持从算法仿真直接迁移到真实调制解调器部署，是工业级水声网络开发的首选平台 |
| **EvoLogics 硬件用户** | EviNS Framework | 原生支持 EvoLogics 调制解调器，含 ROS 集成和 Docker 部署方案 |
| **深度学习方向** | UWSL-APP | 目前开源水声定位中唯一基于神经网络的方法，适合探索 AI 驱动的水声定位新范式 |

---

## 七、总结

水声定位开源生态在 2025-2026 年迎来了一波显著增长，尤其是 Raspi²USBL（2025 年）和 USBL-Simulator（2025 年）填补了 USBL 方向的开源空白。UCNLNav 持续更新（2026 年 7 月）成为最全面的导航算法库，而 UnetStack 和 EviNS 则提供了从仿真到部署的工业级平台。

从技术趋势来看，**三个方向值得关注**：

1. **USBL 系统的低成本化** — 树莓派方案大幅降低了 USBL 系统的硬件门槛
2. **深度学习在声源定位中的应用** — UWSL-APP 代表了 AI 驱动的新范式
3. **仿真与实测的深度融合** — ROS2/UnetStack 使从仿真到部署的迁移更加平滑

对于研究者和工程师而言，当前已有足够的开源资源支撑从算法学习到系统开发的全流程。

---

## 参考资料

1. UnetStack, Underwater Networks Handbook — 水声网络基础理论与定位方法。https://unetstack.net/handbook/unet-handbook.html
2. EviNS Framework, GitHub — EvoLogics 水下声学传感器网络与定位系统开发框架。https://github.com/EvoLogics/evins
3. UnderwaterAcousticTracker, GitHub — SIO Jaffe Lab 基于 TDOA/TOA 的水下声学追踪器。https://github.com/SIOJaffeLab/UnderwaterAcousticTracker
4. Huang et al., Raspi²USBL: An open-source Raspberry Pi-Based Passive Inverted Ultra-Short Baseline Positioning System for Underwater Robotics, arXiv:2511.06998, 2025. https://arxiv.org/pdf/2511.06998
5. UCNLNav, GitHub — 多语言导航算法库（C#/Rust/Matlab），含 TDOA/TOA/AOA/VLBL 算法。https://github.com/ucnl/UCNLNav
6. USBL-Simulator, GitHub — C++/ROS 2 超短基线 USBL 仿真器。https://github.com/maximilian-nitsch/USBL-Simulator
7. Kebkal et al., EviNS: A Framework for Development of Underwater Acoustic Sensor Networks and Positioning Systems, Erlang Factory 2015. https://www.erlang-factory.com/static/upload/media/1434462754487829okebkaleuc2015.pdf
8. Chitre et al., UnetStack: an Agent-based Software Stack and Simulator for Underwater Networks, OCEANS 2014. https://arl.nus.edu.sg/wp-content/publications/Oceans14unetstack.pdf
9. UnetStack Blog, Turning a Multi-Receiver Modem into a USBL Transceiver — USBL 算法实现教程。https://blog.unetstack.net/turning-a-multi-receiver-modem-into-a-usbl-transceiver
10. UWSL-APP, GitHub — 基于神经网络的水下声源定位应用。https://github.com/Perry44001/UWSL-APP
11. WHOI Micro-Modem, Underwater Acoustic Navigation — 支持 LBL 导航和 OWTT 测距的声学调制解调器。https://deepblue.lib.umich.edu/bitstreams/c1ff175e-6fef-498d-bd65-b5b45153e30d/download
12. Three-Dimensional Ultra-Short Base Line Based Underwater Acoustical Localization Utilizing Modified Newton Algorithm, IEEE, 2021. https://xplorestaging.ieee.org/ielx7/6287639/9312710/09445010.pdf
13. GAS Tightly Coupled LBL/USBL Position and Velocity Filter for Underwater Vehicles, ISR/IST Lisbon. http://welcome.isr.ist.utl.pt/wp-content/uploads/2015/05/3211_C40.pdf
