# Underwater Acoustics Learning

水声学开源学习平台，面向水声传播、声呐信号处理、水声通信、被动声学监测、数据集与工程工具链的系统化整理。

本项目参考优秀导航学习仓库 [Navigation-Learning](https://github.com/LiZhengXiao99/Navigation-Learning) 的组织方式，但内容聚焦水声学与海洋声学。目标不是简单堆链接，而是把可复现、可阅读、可二次开发的开源资源整理成一条学习路线。

## 学习地图

1. 基础理论：声速剖面、传播损失、射线/简正波/抛物方程、混响与噪声。
2. 传播建模：BELLHOP、KRAKEN、SCOOTER、RAM、3D 射线追踪与环境建模。
3. 阵列与声呐：波束形成、DOA、匹配场处理、主动/被动声呐、目标强度。
4. 水声通信：信道建模、调制解调、网络协议、仿真平台。
5. 数据与智能：船舶辐射噪声、生物声学、被动声学监测、深度学习识别。
6. 工程实践：MATLAB/Python/Julia 工具链、可视化、验证数据、论文复现。

## 仓库内容

| 模块 | 说明 |
| --- | --- |
| [开源项目记录](docs/开源项目记录.md) | 按方向整理水声相关开源项目、工具箱、仿真平台 |
| [开源数据集记录](docs/开源数据集记录.md) | 船舶噪声、生物声学、海洋声学与声呐相关数据 |
| [书籍讲义课程](docs/书籍讲义课程.md) | 课程、讲义、教材、论文综述与入门材料 |
| [常用网站与工具](docs/常用网站与工具.md) | OALIB、NOAA、海洋环境数据、可视化工具 |
| [源码阅读计划](docs/源码阅读计划.md) | 建议优先精读的项目和阅读路线 |
| [GitHub 发布指南](docs/GitHub发布指南.md) | 创建远程仓库、首次提交与维护建议 |

## 首批推荐

| 方向 | 推荐资源 | 为什么值得看 |
| --- | --- | --- |
| 水声传播 | [Acoustics Toolbox](https://oalib-acoustics.org/website_resources/AcousticsToolbox/) | BELLHOP、KRAKEN、SCOOTER 等经典模型入口 |
| Python 工具 | [arlpy](https://github.com/org-arl/arlpy) | 包含 underwater acoustics、beamforming、signal processing |
| Julia 工具 | [UnderwaterAcoustics.jl](https://github.com/org-arl/UnderwaterAcoustics.jl) | 现代 Julia 水声建模接口，适合学习抽象设计 |
| 通信网络 | [DESERT Underwater](https://github.com/signetlabdei/DESERT_Underwater) | 水声网络仿真经典开源框架 |
| 通信网络 | [Aqua-Sim-NG](https://github.com/rmartin5/aqua-sim-ng) | ns-3 下的水声网络仿真模块 |
| 被动声学 | [PAMGuard](https://github.com/PAMGuard/PAMGuard) | 被动声学监测与海洋哺乳动物检测工具 |
| 生物声学 AI | [Ketos](https://github.com/meridian-acoustics/ketos) | 面向水下声学数据的机器学习工具 |
| 通用声学 AI | [OpenSoundscape](https://github.com/kitzeslab/opensoundscape) | 生物声学/声景分析，可迁移到水声数据处理 |

## 贡献方式

欢迎提交 Issue 或 Pull Request。新增资源请尽量包含：

- 项目名称与链接
- 所属方向
- 主要语言/平台
- 开源许可证
- 一句话学习价值
- 适合入门、进阶还是工程复现

详见 [CONTRIBUTING.md](CONTRIBUTING.md)。

## 许可证说明

本仓库整理性文字内容采用 [CC BY 4.0](LICENSE) 共享；各链接项目、数据集、论文和课程遵守其原始许可证或使用条款。
