<div align="center">

# 🌊 Underwater Acoustics Learning

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](LICENSE)
[![Stars](https://img.shields.io/github/stars/SatelliteCoder/Underwater-Acoustics-Learning?style=flat&logo=github&label=Stars)](https://github.com/SatelliteCoder/Underwater-Acoustics-Learning/stargazers)
[![Forks](https://img.shields.io/github/forks/SatelliteCoder/Underwater-Acoustics-Learning?style=flat&logo=github&label=Forks)](https://github.com/SatelliteCoder/Underwater-Acoustics-Learning/network/members)
[![Last Commit](https://img.shields.io/github/last-commit/SatelliteCoder/Underwater-Acoustics-Learning?style=flat&label=Last%20Commit)](https://github.com/SatelliteCoder/Underwater-Acoustics-Learning/commits)
[![Code Size](https://img.shields.io/github/languages/code-size/SatelliteCoder/Underwater-Acoustics-Learning?style=flat&label=Code%20Size)](https://github.com/SatelliteCoder/Underwater-Acoustics-Learning)
[![Topic](https://img.shields.io/badge/Topic-Ocean%20Acoustics-blue)](https://github.com/SatelliteCoder/Underwater-Acoustics-Learning)
[![Tech](https://img.shields.io/badge/Tech-Python%20%7C%20Julia-green)](https://github.com/SatelliteCoder/Underwater-Acoustics-Learning)
[![Status](https://img.shields.io/badge/Status-Active-brightgreen)](https://github.com/SatelliteCoder/Underwater-Acoustics-Learning)

</div>

> 📚 水声学开源学习平台，系统整理水声传播、声场仿真、声呐与感知装备仿真、水声通信、UUV/环境噪声、被动声学监测、水声目标识别、水声定位、水声数据处理、信号增强、开源数据集、论文与课程资料。
>
> 本项目内容聚焦 **underwater acoustics / ocean acoustics / sonar**。
> - 资源名称：直接跳转仓库/网站/数据集入口
> - `详情`：跳转仓库内中文解析笔记

---

## 📋 目录
- [🚀 学习路线](#-学习路线)
- [📄 仓库文档](#-仓库文档)
- [🔊 一、声场传播与仿真](#一-声场传播与仿真)
- [🛰️ 二、声呐与感知装备仿真](#二-声呐与感知装备仿真)
- [📊 三、水声数据处理与可视化](#三-水声数据处理与可视化)
- [🌫️ 四、UUV 与环境噪声、声景分析](#四-uuv-与环境噪声声景分析)
- [📡 五、水声通信、网络与定位](#五-水声通信网络与定位)
- [🤖 六、目标识别与机器学习](#六-目标识别与机器学习)
- [🎛️ 七、信号增强、阵列处理与声学 DSP](#七-信号增强阵列处理与声学-dsp)
- [🗂️ 八、开放数据集与环境数据](#八-开放数据集与环境数据)
- [📜 九、论文、标准与专题资料](#九-论文标准与专题资料)
- [🤝 贡献方式](#-贡献方式)
- [©️ 许可证说明](#️-许可证说明)

---

## 🚀 学习路线

<table width="100%">
  <tr>
    <th width="18%">阶段</th>
    <th width="47%">核心问题</th>
    <th width="35%">推荐入口</th>
  </tr>
  <tr>
    <td>1. 基础概念</td>
    <td>声压、声强、传播损失、声呐方程、声速剖面</td>
    <td><a href="docs/水声学原理概念参数原理汇总.md">水声学原理概念参数原理汇总</a></td>
  </tr>
  <tr>
    <td>2. 声场建模</td>
    <td>射线、简正波、抛物方程、海底/海面边界</td>
    <td><a href="#一-声场传播与仿真">声场传播与仿真</a></td>
  </tr>
  <tr>
    <td>3. 声呐感知</td>
    <td>主动/被动声呐、多波束、水柱、侧扫、成像声呐</td>
    <td><a href="#二-声呐与感知装备仿真">声呐与感知装备仿真</a></td>
  </tr>
  <tr>
    <td>4. 数据处理</td>
    <td>echosounder、水柱声呐、NetCDF、声景长期统计</td>
    <td><a href="#三-水声数据处理与可视化">水声数据处理与可视化</a></td>
  </tr>
  <tr>
    <td>5. 智能识别</td>
    <td>船舶辐射噪声、海洋哺乳动物、目标识别、事件检测</td>
    <td><a href="#六-目标识别与机器学习">目标识别与机器学习</a></td>
  </tr>
  <tr>
    <td>6. 工程系统</td>
    <td>水声通信、定位、UUV 仿真、噪声模型、数据集复现</td>
    <td><a href="#五-水声通信网络与定位">通信网络与定位</a></td>
  </tr>
</table>

---

## 📄 仓库文档

> 💡 全部笔记存放在 `docs/` 目录，持续更新维护。

<table width="100%">
  <tr>
    <th width="30%">文档</th>
    <th width="70%">内容说明</th>
  </tr>
  <tr>
    <td><a href="docs/项目详细解析.md">项目详细解析</a></td>
    <td>首页重点项目：用途、学习价值、适用场景、注意事项</td>
  </tr>
  <tr>
    <td><a href="docs/开源项目记录.md">开源项目记录</a></td>
    <td>完整项目清单，适合持续追加新项目</td>
  </tr>
  <tr>
    <td><a href="docs/开源数据集记录.md">开源数据集记录</a></td>
    <td>船舶噪声、生物声学、海洋声学、声呐相关数据集汇总</td>
  </tr>
  <tr>
    <td><a href="docs/论文与综述资料.md">论文与综述资料</a></td>
    <td>工具、数据集、研究方向配套论文、标准、综述入口</td>
  </tr>
  <tr>
    <td><a href="docs/书籍讲义课程.md">书籍讲义课程</a></td>
    <td>教材、网课、讲义与学习材料</td>
  </tr>
  <tr>
    <td><a href="docs/常用网站与工具.md">常用网站与工具</a></td>
    <td>OALIB、NOAA、海洋环境数据、可视化工具集合</td>
  </tr>
  <tr>
    <td><a href="docs/源码阅读计划.md">源码阅读计划</a></td>
    <td>优先精读项目清单与源码阅读路线</td>
  </tr>
  <tr>
    <td><a href="docs/GitHub发布指南.md">GitHub 发布指南</a></td>
    <td>仓库创建、初次提交、项目维护建议</td>
  </tr>
</table>

---

## 🔊 一、声场传播与仿真

<table width="100%">
  <tr>
    <th width="32%">项目/工具</th>
    <th width="16%">类型</th>
    <th width="37%">适合学习什么</th>
    <th width="15%">详情</th>
  </tr>
  <tr>
    <td><a href="https://oalib-acoustics.org/website_resources/AcousticsToolbox/">Acoustics Toolbox</a></td>
    <td>经典水声模型工具箱</td>
    <td>BELLHOP、KRAKEN、SCOOTER、SPARC 传播模型</td>
    <td><a href="docs/项目详细解析.md#acoustics-toolbox">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/org-arl/arlpy">arlpy</a></td>
    <td>Python 水声/阵列工具</td>
    <td>BELLHOP调用、水声传播、波束形成</td>
    <td><a href="docs/项目详细解析.md#arlpy">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/org-arl/UnderwaterAcoustics.jl">UnderwaterAcoustics.jl</a></td>
    <td>Julia 水声建模框架</td>
    <td>环境对象、传播模型接口、现代科学计算抽象</td>
    <td><a href="docs/项目详细解析.md#underwateracousticsjl">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/org-arl/AcousticsToolbox.jl">AcousticsToolbox.jl</a></td>
    <td>Julia 封装库</td>
    <td>Julia环境调用 Acoustics Toolbox</td>
    <td><a href="docs/项目详细解析.md#acousticstoolboxjl">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/org-arl/AcousticRayTracers.jl">AcousticRayTracers.jl</a></td>
    <td>射线追踪库</td>
    <td>几何声学、射线轨迹、到达结构分析</td>
    <td><a href="docs/项目详细解析.md#acousticraytracersjl">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/org-arl/VirtualAcousticOcean.jl">VirtualAcousticOcean.jl</a></td>
    <td>虚拟声学海洋</td>
    <td>环境场、声源、接收器一体化仿真搭建</td>
    <td><a href="docs/项目详细解析.md#virtualacousticoceanjl">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/A-New-BellHope/bellhopcuda">bellhopcuda</a></td>
    <td>BELLHOP GPU加速</td>
    <td>声线模型加速、CUDA并行化实现</td>
    <td><a href="docs/项目详细解析.md#bellhopcuda">详情</a></td>
  </tr>
</table>

---

## 🛰️ 二、声呐与感知装备仿真

<table width="100%">
  <tr>
    <th width="32%">项目/工具</th>
    <th width="16%">类型</th>
    <th width="37%">适合学习什么</th>
    <th width="15%">详情</th>
  </tr>
  <tr>
    <td><a href="https://github.com/uuvsimulator/uuv_simulator">UUV Simulator</a></td>
    <td>ROS/Gazebo UUV仿真</td>
    <td>水下机器人、传感器插件、任务仿真</td>
    <td><a href="docs/项目详细解析.md#uuv-simulator">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/Field-Robotics-Lab/dave">DAVE</a></td>
    <td>水下机器人仿真环境</td>
    <td>UUV动力学、海流、声呐/视觉传感器仿真</td>
    <td><a href="docs/项目详细解析.md#dave">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/AntoineRichard/IsaacSim_Underwater">Isaac Sim Underwater</a></td>
    <td>Isaac Sim水下仿真</td>
    <td>现代机器人仿真、水下声学视觉扩展</td>
    <td><a href="docs/项目详细解析.md#isaac-sim-underwater">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/patrykcieslak/stonefish">Stonefish</a></td>
    <td>海洋机器人仿真库</td>
    <td>水下动力学、传感器、机器人任务仿真</td>
    <td><a href="docs/项目详细解析.md#stonefish">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/Field-Robotics-Lab/sonar_simulation">sonar_simulation</a></td>
    <td>成像声呐仿真</td>
    <td>Gazebo/ROS前视声呐数据生成</td>
    <td><a href="docs/项目详细解析.md#sonar-simulation">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/RobustFieldAutonomyLab/sonar-litreview">sonar-litreview</a></td>
    <td>声呐文献索引</td>
    <td>成像声呐、声呐SLAM、感知算法资料入口</td>
    <td><a href="docs/项目详细解析.md#sonar-litreview">详情</a></td>
  </tr>
</table>

---

## 📊 三、水声数据处理与可视化

<table width="100%">
  <tr>
    <th width="32%">项目/工具</th>
    <th width="16%">类型</th>
    <th width="37%">适合学习什么</th>
    <th width="15%">详情</th>
  </tr>
  <tr>
    <td><a href="https://github.com/alexschimel/Espresso">Espresso</a></td>
    <td>水柱声呐可视化</td>
    <td>多波束水体数据、垂直回声积分、异常可视化</td>
    <td><a href="docs/项目详细解析.md#espresso">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/alexschimel/CoFFee">CoFFee</a></td>
    <td>多波束/水柱处理工具箱</td>
    <td>Kongsberg多波束文件解析、水柱数据读取处理</td>
    <td><a href="docs/项目详细解析.md#coffee">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://www.ncei.noaa.gov/maps/water-column-sonar/">NOAA Water Column Sonar Viewer</a></td>
    <td>水柱声呐数据地图</td>
    <td>浏览、下载NCEI水柱声呐公开数据</td>
    <td><a href="docs/项目详细解析.md#noaa-water-column-sonar-viewer">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://registry.opendata.aws/ncei-wcsd-archive/">NCEI Water Column Sonar Data on AWS</a></td>
    <td>开放数据归档</td>
    <td>获取大规模水柱声呐原始数据集</td>
    <td><a href="docs/项目详细解析.md#ncei-wcsd-aws">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/OSOceanAcoustics/echopype">echopype</a></td>
    <td>echosounder数据处理</td>
    <td>回声测深数据标准化转换</td>
    <td><a href="docs/项目详细解析.md#echopype">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/noaa-afsc-mace/pyEcholab">pyEcholab</a></td>
    <td>NOAA回声测深处理</td>
    <td>EK60/EK80渔业声学数据读取处理</td>
    <td><a href="docs/项目详细解析.md#pyecholab">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/dwcaress/MB-System">MB-System</a></td>
    <td>多波束测深处理</td>
    <td>海底地形、多波束处理、海洋测绘工具链</td>
    <td><a href="docs/项目详细解析.md#mb-system">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/pydata/xarray">xarray</a></td>
    <td>多维科学数据库</td>
    <td>NetCDF、海洋场、声场网格与时序数据处理</td>
    <td><a href="docs/项目详细解析.md#xarray">详情</a></td>
  </tr>
</table>

---

## 🌫️ 四、UUV 与环境噪声、声景分析

<table width="100%">
  <tr>
    <th width="32%">项目/工具</th>
    <th width="16%">类型</th>
    <th width="37%">适合学习什么</th>
    <th width="15%">详情</th>
  </tr>
  <tr>
    <td><a href="https://github.com/PAMGuard/PAMGuard">PAMGuard</a></td>
    <td>被动声学监测平台</td>
    <td>声学事件检测、海洋哺乳动物监测、PAM完整流程</td>
    <td><a href="docs/项目详细解析.md#pamguard">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://bitbucket.org/CLO-BRP/manta-wiki/wiki/Home">MANTA Wiki</a></td>
    <td>海洋声景分析</td>
    <td>长期噪声趋势、标准化声级统计方案</td>
    <td><a href="docs/项目详细解析.md#manta">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/NEFSC/READ-PSB-Marina">Marina</a></td>
    <td>PAM工具集合</td>
    <td>NOAA/NEFSC被动声学常用工具集成</td>
    <td><a href="docs/项目详细解析.md#marina">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/MarineBioAcousticsRC">MarineBioAcousticsRC</a></td>
    <td>生物声学组织</td>
    <td>Tethys、MANTA、Triton海洋生物声学工具合集</td>
    <td><a href="docs/项目详细解析.md#marinebioacousticsrc">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/MarineBioAcousticsRC/Tethys">Tethys</a></td>
    <td>声学元数据管理</td>
    <td>被动声学数据库、检测结果与元数据管理</td>
    <td><a href="docs/项目详细解析.md#tethys">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/meridian-acoustics/ketos">Ketos</a></td>
    <td>水下声学机器学习</td>
    <td>声谱图切片、数据集构建、深度学习检测</td>
    <td><a href="docs/项目详细解析.md#ketos">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/kitzeslab/opensoundscape">OpenSoundscape</a></td>
    <td>声景机器学习</td>
    <td>生物声学深度学习，可迁移水声事件检测</td>
    <td><a href="docs/项目详细解析.md#opensoundscape">详情</a></td>
  </tr>
</table>

---

## 📡 五、水声通信、网络与定位

<table width="100%">
  <tr>
    <th width="32%">项目/工具</th>
    <th width="16%">类型</th>
    <th width="37%">适合学习什么</th>
    <th width="15%">详情</th>
  </tr>
  <tr>
    <td><a href="https://github.com/signetlabdei/DESERT_Underwater">DESERT Underwater</a></td>
    <td>水声网络仿真</td>
    <td>物理层、MAC、路由，ns-2水声网络仿真</td>
    <td><a href="docs/项目详细解析.md#desert-underwater">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/signetlabdei/WOSS">WOSS</a></td>
    <td>海洋环境网络仿真</td>
    <td>环境数据库、声传播-网络仿真耦合</td>
    <td><a href="docs/项目详细解析.md#woss">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/rmartin5/aqua-sim-ng">Aqua-Sim-NG</a></td>
    <td>ns-3水声网络</td>
    <td>水声网络协议仿真与性能评估</td>
    <td><a href="docs/项目详细解析.md#aqua-sim-ng">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/org-arl/unet-contrib">UnetStack contrib</a></td>
    <td>水声网络协议栈</td>
    <td>水声网络协议、仿真、modem接口扩展</td>
    <td><a href="docs/项目详细解析.md#unetstack">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://www3.tuhh.de/acps/projects/ahoi/resources_git/">AHOI modem</a></td>
    <td>开源水声modem</td>
    <td>低成本水声通信硬件、固件、实验接口</td>
    <td><a href="docs/项目详细解析.md#ahoi-modem">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/bensherlock/nm3-python-driver">NM3 Python driver</a></td>
    <td>水声modem驱动</td>
    <td>Modem串口协议、虚拟网络、测试脚本</td>
    <td><a href="docs/项目详细解析.md#nm3-python-driver">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/GSO-soslab/Raspi2USBL">Raspi2USBL</a></td>
    <td>USBL定位实验</td>
    <td>低成本声学定位硬件，树莓派工程实现思路</td>
    <td><a href="docs/项目详细解析.md#raspi2usbl">详情</a></td>
  </tr>
</table>

---

## 🤖 六、目标识别与机器学习

<table width="100%">
  <tr>
    <th width="32%">项目/工具</th>
    <th width="16%">类型</th>
    <th width="37%">适合学习什么</th>
    <th width="15%">详情</th>
  </tr>
  <tr>
    <td><a href="https://github.com/irfankamboh/DeepShip">DeepShip</a></td>
    <td>船舶噪声数据集基准</td>
    <td>水下船型分类、深度学习识别基线</td>
    <td><a href="docs/项目详细解析.md#deepship">详情</a></td>
  </tr>
  <tr>
    <td><a href="http://atlanttic.uvigo.es/underwaternoise/">ShipsEar</a></td>
    <td>船舶辐射噪声数据集</td>
    <td>船舶声纹分类、特征提取、基准实验</td>
    <td><a href="docs/项目详细解析.md#shipsear">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/meridian-acoustics/ketos">Ketos</a></td>
    <td>水声AI工具包</td>
    <td>水下声学检测、分类模型训练流水线</td>
    <td><a href="docs/项目详细解析.md#ketos">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/kitzeslab/opensoundscape">OpenSoundscape</a></td>
    <td>声景AI工具包</td>
    <td>迁移学习、声谱图分类、生态声学检测</td>
    <td><a href="docs/项目详细解析.md#opensoundscape">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/scikit-maad/scikit-maad">scikit-maad</a></td>
    <td>声景特征工具</td>
    <td>声学指数、时频特征、生态声学分析</td>
    <td><a href="docs/项目详细解析.md#scikit-maad">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/librosa/librosa">librosa</a></td>
    <td>音频特征基础库</td>
    <td>MFCC、谱图、频谱特征，水声预处理基础</td>
    <td><a href="docs/项目详细解析.md#librosa">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/pytorch/audio">torchaudio</a></td>
    <td>深度学习音频库</td>
    <td>PyTorch音频增强、分类、声谱图前端模块</td>
    <td><a href="docs/项目详细解析.md#torchaudio">详情</a></td>
  </tr>
</table>

---

## 🎛️ 七、信号增强、阵列处理与声学 DSP

<table width="100%">
  <tr>
    <th width="32%">项目/工具</th>
    <th width="16%">类型</th>
    <th width="37%">适合学习什么</th>
    <th width="15%">详情</th>
  </tr>
  <tr>
    <td><a href="https://github.com/org-arl/arlpy">arlpy.bf</a></td>
    <td>阵列波束形成</td>
    <td>Bartlett、Capon、MUSIC，宽窄带波束形成算法</td>
    <td><a href="docs/项目详细解析.md#arlpy">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/LCAV/pyroomacoustics">pyroomacoustics</a></td>
    <td>声学阵列/DSP库</td>
    <td>DOA估计、波束形成、STFT，可迁移水声定位</td>
    <td><a href="docs/项目详细解析.md#pyroomacoustics">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/acoular/acoular">Acoular</a></td>
    <td>阵列声源定位库</td>
    <td>波束形成、声源成像、阵列处理工程框架</td>
    <td><a href="docs/项目详细解析.md#acoular">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/scipy/scipy">scipy.signal</a></td>
    <td>通用信号处理</td>
    <td>滤波、谱估计、相关、STFT、检测基础算法</td>
    <td><a href="docs/项目详细解析.md#scipysignal">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/timsainb/noisereduce">noisereduce</a></td>
    <td>音频降噪工具</td>
    <td>谱减、噪声门控，水声降噪基线方案</td>
    <td><a href="docs/项目详细解析.md#noisereduce">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/asteroid-team/asteroid">asteroid</a></td>
    <td>深度音频分离框架</td>
    <td>深度学习分离，迁移水声信号增强研究</td>
    <td><a href="docs/项目详细解析.md#asteroid">详情</a></td>
  </tr>
</table>

---

## 🗂️ 八、开放数据集与环境数据

<table width="100%">
  <tr>
    <th width="32%">数据/网站</th>
    <th width="16%">类型</th>
    <th width="37%">适合学习什么</th>
    <th width="15%">详情</th>
  </tr>
  <tr>
    <td><a href="https://www.fisheries.noaa.gov/national/science-data/passive-acoustic-data">NOAA Passive Acoustic Data</a></td>
    <td>被动声学数据入口</td>
    <td>海洋声景、长期监测项目数据检索</td>
    <td><a href="docs/项目详细解析.md#noaa-passive-acoustic-data">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://cis.whoi.edu/science/B/whalesounds/">Watkins Marine Mammal Sound Database</a></td>
    <td>海洋哺乳动物声音库</td>
    <td>生物声学识别、动物叫声检测</td>
    <td><a href="docs/项目详细解析.md#watkins-database">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://www.soest.hawaii.edu/ore/dclde/">DCLDE</a></td>
    <td>检测分类定位数据集</td>
    <td>海洋哺乳动物检测、分类、定位基准数据集</td>
    <td><a href="docs/项目详细解析.md#dclde">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://argo.ucsd.edu/">Argo</a></td>
    <td>温盐深剖面</td>
    <td>声速剖面构建、传播环境搭建</td>
    <td><a href="docs/项目详细解析.md#argo">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://marine.copernicus.eu/">Copernicus Marine</a></td>
    <td>海洋再分析/预报</td>
    <td>三维温盐深、海流、海洋环境场获取</td>
    <td><a href="docs/项目详细解析.md#copernicus-marine">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://www.gebco.net/">GEBCO</a></td>
    <td>全球海底地形</td>
    <td>海底边界建模、声传播场景构建</td>
    <td><a href="docs/项目详细解析.md#gebco">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://www.teos-10.org/software.htm">TEOS-10</a></td>
    <td>海水状态方程工具</td>
    <td>声速、密度、温盐深物理参数计算</td>
    <td><a href="docs/项目详细解析.md#teos-10">详情</a></td>
  </tr>
</table>

---

## 📜 九、论文、标准与专题资料

<table width="100%">
  <tr>
    <th width="32%">资料</th>
    <th width="16%">类型</th>
    <th width="37%">适合学习什么</th>
    <th width="15%">详情</th>
  </tr>
  <tr>
    <td><a href="https://oalib-acoustics.org/">Ocean Acoustic Library</a></td>
    <td>模型资料库</td>
    <td>水声传播模型、测试算例、经典学习资料入口</td>
    <td><a href="docs/项目详细解析.md#ocean-acoustic-library">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://www.iso.org/standard/62406.html">ISO 18405 Underwater Acoustics Terminology</a></td>
    <td>国际标准</td>
    <td>水下声学术语、声景测量规范表述</td>
    <td><a href="docs/论文与综述资料.md#iso-18405">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://bitbucket.org/CLO-BRP/manta-wiki/wiki/Home">MANTA Wiki</a></td>
    <td>工具论文指南</td>
    <td>海洋声景标准化处理建议文档</td>
    <td><a href="docs/论文与综述资料.md#manta">详情</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/RobustFieldAutonomyLab/sonar-litreview">sonar-litreview</a></td>
    <td>文献索引</td>
    <td>成像声呐、声呐SLAM、水下机器人感知论文集合</td>
    <td><a href="docs/项目详细解析.md#sonar-litreview">详情</a></td>
  </tr>
</table>

---

## 🤝 贡献方式

欢迎提交 Issue 或 Pull Request。新增资源尽量包含下面信息：

- 项目名称与链接
- 所属研究方向
- 主要语言 / 运行平台
- 开源许可证或数据集使用条款
- 一句话学习价值
- 标签：入门 / 进阶 / 工程复现 / 研究复现

详见 [CONTRIBUTING.md](CONTRIBUTING.md)。

---

## ©️ 许可证说明

本仓库整理的文字内容采用 [CC BY 4.0](LICENSE) 协议共享；
外部链接指向的项目、数据集、论文、课程，请遵守其原始许可证与使用条款。
