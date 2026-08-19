# Underwater Acoustics Learning

[![Link check](https://github.com/SatelliteCoder/Underwater-Acoustics-Learning/actions/workflows/link-check.yml/badge.svg)](https://github.com/SatelliteCoder/Underwater-Acoustics-Learning/actions/workflows/link-check.yml)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](LICENSE)

水声学开源学习平台，系统整理水声传播、声场仿真、声呐与感知装备仿真、水声通信、UUV/环境噪声、被动声学监测、水声目标识别、水声定位、水声数据处理、信号增强、数据集、论文与课程资料。

本项目参考 [Navigation-Learning](https://github.com/LiZhengXiao99/Navigation-Learning) 的学习型仓库组织方式，但内容聚焦 underwater acoustics / ocean acoustics / sonar。资源名称可直接跳转到对应仓库、网站或数据入口；“详情”会跳转到仓库内的中文解析笔记。

## 学习路线

| 阶段 | 核心问题 | 推荐入口 |
| --- | --- | --- |
| 1. 基础概念 | 声压、声强、传播损失、声呐方程、声速剖面 | [水声学原理概念参数原理汇总](docs/水声学原理概念参数原理汇总.md) |
| 2. 声场建模 | 射线、简正波、抛物方程、海底/海面边界 | [声场传播与仿真](#一声场传播与仿真) |
| 3. 声呐感知 | 主动/被动声呐、多波束、水柱、侧扫、成像声呐 | [声呐与感知装备仿真](#二声呐与感知装备仿真) |
| 4. 数据处理 | echosounder、水柱声呐、NetCDF、声景长期统计 | [水声数据处理与可视化](#三水声数据处理与可视化) |
| 5. 智能识别 | 船舶辐射噪声、海洋哺乳动物、目标识别、事件检测 | [目标识别与机器学习](#六目标识别与机器学习) |
| 6. 工程系统 | 水声通信、定位、UUV 仿真、噪声模型、数据集复现 | [通信网络与定位](#五水声通信网络与定位) |

## 仓库文档

| 文档 | 内容 |
| --- | --- |
| [项目详细解析](docs/项目详细解析.md) | 首页所有重点项目的用途、学习价值、适用场景和注意事项 |
| [开源项目记录](docs/开源项目记录.md) | 较完整的项目清单，适合持续追加 |
| [开源数据集记录](docs/开源数据集记录.md) | 船舶噪声、生物声学、海洋声学与声呐相关数据 |
| [论文与综述资料](docs/论文与综述资料.md) | 与工具、数据集和方向相关的论文/标准/综述入口 |
| [书籍讲义课程](docs/书籍讲义课程.md) | 教材、课程、讲义和学习材料 |
| [常用网站与工具](docs/常用网站与工具.md) | OALIB、NOAA、海洋环境数据、可视化工具 |
| [源码阅读计划](docs/源码阅读计划.md) | 建议优先精读的项目和阅读路线 |
| [GitHub 发布指南](docs/GitHub发布指南.md) | 创建远程仓库、首次提交与维护建议 |

## 一、声场传播与仿真

| 项目/工具 | 类型 | 适合学习什么 | 详情 |
| --- | --- | --- | --- |
| [Acoustics Toolbox](https://oalib-acoustics.org/website_resources/AcousticsToolbox/) | 经典水声模型工具箱 | BELLHOP、KRAKEN、SCOOTER、SPARC 等传播模型 | [详情](docs/项目详细解析.md#acoustics-toolbox) |
| [arlpy](https://github.com/org-arl/arlpy) | Python 水声/阵列工具 | BELLHOP 调用、水声传播、波束形成 | [详情](docs/项目详细解析.md#arlpy) |
| [UnderwaterAcoustics.jl](https://github.com/org-arl/UnderwaterAcoustics.jl) | Julia 水声建模框架 | 环境对象、传播模型接口、现代科学计算抽象 | [详情](docs/项目详细解析.md#underwateracousticsjl) |
| [AcousticsToolbox.jl](https://github.com/org-arl/AcousticsToolbox.jl) | Julia 封装 | 在 Julia 中调用 Acoustics Toolbox | [详情](docs/项目详细解析.md#acousticstoolboxjl) |
| [AcousticRayTracers.jl](https://github.com/org-arl/AcousticRayTracers.jl) | 射线追踪 | 几何声学、射线轨迹、到达结构 | [详情](docs/项目详细解析.md#acousticraytracersjl) |
| [VirtualAcousticOcean.jl](https://github.com/org-arl/VirtualAcousticOcean.jl) | 虚拟声学海洋 | 环境场、声源、接收器与仿真组合 | [详情](docs/项目详细解析.md#virtualacousticoceanjl) |
| [bellhopcuda](https://github.com/A-New-BellHope/bellhopcuda) | BELLHOP GPU 加速 | 声线模型加速、CUDA 并行化 | [详情](docs/项目详细解析.md#bellhopcuda) |

## 二、声呐与感知装备仿真

| 项目/工具 | 类型 | 适合学习什么 | 详情 |
| --- | --- | --- | --- |
| [UUV Simulator](https://github.com/uuvsimulator/uuv_simulator) | ROS/Gazebo UUV 仿真 | 水下机器人、传感器插件、任务仿真 | [详情](docs/项目详细解析.md#uuv-simulator) |
| [DAVE](https://github.com/Field-Robotics-Lab/dave) | 水下机器人仿真环境 | UUV 动力学、海流、声呐/视觉传感器仿真 | [详情](docs/项目详细解析.md#dave) |
| [Isaac Sim Underwater](https://github.com/AntoineRichard/IsaacSim_Underwater) | Isaac Sim 水下仿真 | 现代机器人仿真、传感器和水下视觉声学扩展 | [详情](docs/项目详细解析.md#isaac-sim-underwater) |
| [Stonefish](https://github.com/patrykcieslak/stonefish) | 海洋机器人仿真库 | 水下动力学、传感器、机器人任务仿真 | [详情](docs/项目详细解析.md#stonefish) |
| [sonar_simulation](https://github.com/Field-Robotics-Lab/sonar_simulation) | 成像声呐仿真 | Gazebo/ROS 中的前视声呐数据生成 | [详情](docs/项目详细解析.md#sonar-simulation) |
| [sonar-litreview](https://github.com/RobustFieldAutonomyLab/sonar-litreview) | 声呐文献与资源索引 | 成像声呐、声呐 SLAM、感知算法资料入口 | [详情](docs/项目详细解析.md#sonar-litreview) |

## 三、水声数据处理与可视化

| 项目/工具 | 类型 | 适合学习什么 | 详情 |
| --- | --- | --- | --- |
| [Espresso](https://github.com/alexschimel/Espresso) | 水柱声呐可视化 | 多波束水体数据处理、垂直回声积分、异常可视化 | [详情](docs/项目详细解析.md#espresso) |
| [CoFFee](https://github.com/alexschimel/CoFFee) | 多波束/水柱处理工具箱 | Kongsberg 多波束文件解析、水柱数据读取与处理 | [详情](docs/项目详细解析.md#coffee) |
| [NOAA Water Column Sonar Viewer](https://www.ncei.noaa.gov/maps/water-column-sonar/) | 水柱声呐数据地图 | 查看和下载 NCEI 水柱声呐数据 | [详情](docs/项目详细解析.md#noaa-water-column-sonar-viewer) |
| [NCEI Water Column Sonar Data on AWS](https://registry.opendata.aws/ncei-wcsd-archive/) | 开放数据归档 | 大规模水柱声呐原始数据获取 | [详情](docs/项目详细解析.md#ncei-wcsd-aws) |
| [echopype](https://github.com/OSOceanAcoustics/echopype) | echosounder 数据处理 | 声学回声测深数据转标准化科学数据格式 | [详情](docs/项目详细解析.md#echopype) |
| [pyEcholab](https://github.com/noaa-afsc-mace/pyEcholab) | NOAA 回声测深处理 | EK60/EK80 等渔业声学数据读取与处理 | [详情](docs/项目详细解析.md#pyecholab) |
| [MB-System](https://github.com/dwcaress/MB-System) | 多波束测深处理 | 海底地形、多波束处理、海洋测绘工具链 | [详情](docs/项目详细解析.md#mb-system) |
| [xarray](https://github.com/pydata/xarray) | 多维科学数据 | NetCDF、海洋场、声场网格和时间序列处理 | [详情](docs/项目详细解析.md#xarray) |

## 四、UUV 与环境噪声、声景分析

| 项目/工具 | 类型 | 适合学习什么 | 详情 |
| --- | --- | --- | --- |
| [PAMGuard](https://github.com/PAMGuard/PAMGuard) | 被动声学监测平台 | 声学事件检测、海洋哺乳动物监测、实时 PAM 流程 | [详情](docs/项目详细解析.md#pamguard) |
| [MANTA](https://bitbucket.org/CLO-BRP/manta-wiki/wiki/Home) | 海洋声景分析 | 长期环境噪声趋势、标准化声级统计 | [详情](docs/项目详细解析.md#manta) |
| [Marina](https://github.com/NEFSC/READ-PSB-Marina) | PAM 数据处理工具集合 | NOAA/NEFSC 被动声学常用工具集成 | [详情](docs/项目详细解析.md#marina) |
| [MarineBioAcousticsRC](https://github.com/MarineBioAcousticsRC) | 生物声学工具组织 | Tethys、MANTA、Triton 等海洋生物声学工具 | [详情](docs/项目详细解析.md#marinebioacousticsrc) |
| [Tethys](https://github.com/MarineBioAcousticsRC/Tethys) | 声学元数据管理 | 被动声学数据库、检测结果和元数据组织 | [详情](docs/项目详细解析.md#tethys) |
| [Ketos](https://github.com/meridian-acoustics/ketos) | 水下声学机器学习 | 声谱图、训练数据切片、深度学习检测 | [详情](docs/项目详细解析.md#ketos) |
| [OpenSoundscape](https://github.com/kitzeslab/opensoundscape) | 声景机器学习 | 生物声学深度学习，可迁移到水声事件检测 | [详情](docs/项目详细解析.md#opensoundscape) |

## 五、水声通信、网络与定位

| 项目/工具 | 类型 | 适合学习什么 | 详情 |
| --- | --- | --- | --- |
| [DESERT Underwater](https://github.com/signetlabdei/DESERT_Underwater) | 水声网络仿真 | 物理层、MAC、路由、ns-2 水声网络仿真 | [详情](docs/项目详细解析.md#desert-underwater) |
| [WOSS](https://github.com/signetlabdei/WOSS) | 海洋环境网络仿真 | 环境数据库、声传播与网络仿真耦合 | [详情](docs/项目详细解析.md#woss) |
| [Aqua-Sim-NG](https://github.com/rmartin5/aqua-sim-ng) | ns-3 水声网络 | 水声网络协议仿真和性能评估 | [详情](docs/项目详细解析.md#aqua-sim-ng) |
| [UnetStack contrib](https://github.com/org-arl/unet-contrib) | 水声网络协议栈 | 水声网络协议、仿真、modem 接口扩展 | [详情](docs/项目详细解析.md#unetstack) |
| [AHOI modem](https://www3.tuhh.de/acps/projects/ahoi/resources_git/) | 开源水声 modem | 低成本水声通信硬件、固件与实验接口 | [详情](docs/项目详细解析.md#ahoi-modem) |
| [NM3 Python driver](https://github.com/bensherlock/nm3-python-driver) | 水声 modem 驱动 | modem 串口协议、虚拟网络和测试脚本 | [详情](docs/项目详细解析.md#nm3-python-driver) |
| [Raspi2USBL](https://github.com/GSO-soslab/Raspi2USBL) | USBL 定位实验 | 低成本声学定位硬件和树莓派实现思路 | [详情](docs/项目详细解析.md#raspi2usbl) |

## 六、目标识别与机器学习

| 项目/工具 | 类型 | 适合学习什么 | 详情 |
| --- | --- | --- | --- |
| [DeepShip](https://github.com/irfankamboh/DeepShip) | 船舶噪声数据/基准 | 水下船型分类、深度学习识别 | [详情](docs/项目详细解析.md#deepship) |
| [ShipsEar](http://atlanttic.uvigo.es/underwaternoise/) | 船舶辐射噪声数据集 | 船舶声纹分类、特征提取和基准实验 | [详情](docs/项目详细解析.md#shipsear) |
| [Ketos](https://github.com/meridian-acoustics/ketos) | 水声 AI 工具 | 水下声学检测、分类模型训练 | [详情](docs/项目详细解析.md#ketos) |
| [OpenSoundscape](https://github.com/kitzeslab/opensoundscape) | 声景 AI 工具 | 迁移学习、声谱图分类、生态声学检测 | [详情](docs/项目详细解析.md#opensoundscape) |
| [scikit-maad](https://github.com/scikit-maad/scikit-maad) | 声景特征工具 | 声学指数、时频特征、生态声学分析 | [详情](docs/项目详细解析.md#scikit-maad) |
| [librosa](https://github.com/librosa/librosa) | 音频特征基础库 | MFCC、谱图、节拍/频谱特征，可用于水声预处理 | [详情](docs/项目详细解析.md#librosa) |
| [torchaudio](https://github.com/pytorch/audio) | 深度学习音频库 | PyTorch 音频增强、分类、声谱图前端 | [详情](docs/项目详细解析.md#torchaudio) |

## 七、信号增强、阵列处理与声学 DSP

| 项目/工具 | 类型 | 适合学习什么 | 详情 |
| --- | --- | --- | --- |
| [arlpy.bf](https://github.com/org-arl/arlpy) | 阵列波束形成 | Bartlett、Capon、MUSIC、宽带/窄带波束形成 | [详情](docs/项目详细解析.md#arlpy) |
| [pyroomacoustics](https://github.com/LCAV/pyroomacoustics) | 声学阵列/DSP | DOA、波束形成、STFT、声源定位算法迁移学习 | [详情](docs/项目详细解析.md#pyroomacoustics) |
| [Acoular](https://github.com/acoular/acoular) | 阵列声源定位 | 波束形成、声源成像、阵列处理工程结构 | [详情](docs/项目详细解析.md#acoular) |
| [scipy.signal](https://github.com/scipy/scipy) | 通用信号处理 | 滤波、谱估计、相关、STFT、检测基础算法 | [详情](docs/项目详细解析.md#scipysignal) |
| [noisereduce](https://github.com/timsainb/noisereduce) | 音频降噪 | 谱减/噪声门控思路，可作为水声增强基线 | [详情](docs/项目详细解析.md#noisereduce) |
| [asteroid](https://github.com/asteroid-team/asteroid) | 深度音频分离 | 深度学习语音分离框架，可迁移到水声增强研究 | [详情](docs/项目详细解析.md#asteroid) |

## 八、开放数据集与环境数据

| 数据/网站 | 类型 | 适合学习什么 | 详情 |
| --- | --- | --- | --- |
| [NOAA Passive Acoustic Data](https://www.fisheries.noaa.gov/national/science-data/passive-acoustic-data) | 被动声学数据入口 | 海洋声景、长期监测、项目数据发现 | [详情](docs/项目详细解析.md#noaa-passive-acoustic-data) |
| [Watkins Marine Mammal Sound Database](https://cis.whoi.edu/science/B/whalesounds/) | 海洋哺乳动物声音 | 生物声学识别、叫声检测 | [详情](docs/项目详细解析.md#watkins-database) |
| [DCLDE](https://www.soest.hawaii.edu/ore/dclde/) | 检测分类定位数据 | 海洋哺乳动物检测、分类、定位基准 | [详情](docs/项目详细解析.md#dclde) |
| [Argo](https://argo.ucsd.edu/) | 温盐深剖面 | 声速剖面生成和传播环境构建 | [详情](docs/项目详细解析.md#argo) |
| [Copernicus Marine](https://marine.copernicus.eu/) | 海洋再分析/预报 | 三维温盐深、海流和环境场 | [详情](docs/项目详细解析.md#copernicus-marine) |
| [GEBCO](https://www.gebco.net/) | 全球海底地形 | 海底边界和声传播场景 | [详情](docs/项目详细解析.md#gebco) |
| [TEOS-10](https://www.teos-10.org/software.htm) | 海水状态方程工具 | 声速、密度、温盐深物理参数计算 | [详情](docs/项目详细解析.md#teos-10) |

## 九、论文、标准与专题资料

| 资料 | 类型 | 适合学习什么 | 详情 |
| --- | --- | --- | --- |
| [Ocean Acoustic Library](https://oalib-acoustics.org/) | 模型与资料库 | 水声传播模型、测试算例、经典资料入口 | [详情](docs/项目详细解析.md#ocean-acoustic-library) |
| [ISO 18405 Underwater Acoustics Terminology](https://www.iso.org/standard/62406.html) | 标准 | 水下声学术语、声景和测量表述规范 | [详情](docs/论文与综述资料.md#iso-18405) |
| [MANTA wiki](https://bitbucket.org/CLO-BRP/manta-wiki/wiki/Home) | 工具论文/指南入口 | 海洋声景标准化处理建议 | [详情](docs/论文与综述资料.md#manta) |
| [sonar-litreview](https://github.com/RobustFieldAutonomyLab/sonar-litreview) | 文献索引 | 成像声呐、声呐 SLAM、机器人感知论文 | [详情](docs/项目详细解析.md#sonar-litreview) |

## 贡献方式

欢迎提交 Issue 或 Pull Request。新增资源请尽量包含：

- 项目名称与链接
- 所属方向
- 主要语言/平台
- 开源许可证或数据使用条款
- 一句话学习价值
- 适合入门、进阶、工程复现还是研究复现

详见 [CONTRIBUTING.md](CONTRIBUTING.md)。

## 许可证说明

本仓库整理性文字内容采用 [CC BY 4.0](LICENSE) 共享；各链接项目、数据集、论文和课程遵守其原始许可证或使用条款。
