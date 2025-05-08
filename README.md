# 🐾 云深处Lite3机器狗巡检系统

本项目基于云深处 Lite3 机器狗平台，集成海康云台与自研视觉识别服务，实现室内/园区级智能巡检能力。系统模块包括硬件控制、视觉识别、SLAM 建图、自主导航和平台可视化界面。

---

## 🧠 项目功能

- 🔍 视觉识别：支持火焰、人员、安全帽等目标识别
- 🗺️ SLAM 建图：构建室内空间地图
- 🚶 自主导航：巡检路径规划与避障行驶
- 🎥 云台控制：对接海康 PTZ 云台，支持巡航、变焦控制
- 📊 巡检平台：任务配置、数据可视化、事件告警

---

## 📁 仓库结构说明

| 目录 | 描述 |
|------|------|
| `hardware_control/` | 包含机器人本体与海康云台控制接口封装 |
| `vision_module/` | 视觉算法模块，包含检测模型和 API 服务 |
| `slam_navigation/` | 基于 ROS 的 SLAM 与导航控制模块 |
| `platform/` | 巡检平台 Web 可视化系统（前端 + 后端） |
| `config/` | 配置文件（相机参数、导航参数等） |
| `scripts/` | 启动脚本与辅助工具（如相机标定） |
| `tests/` | 单元测试与集成测试代码 |
| `docs/` | 架构文档与部署说明 |
| `docker/` | Docker 镜像构建与部署配置 |

---

## 🚀 快速开始

```bash
git clone https://github.com/your-org/inspection-dog.git
cd inspection-dog
pip install -r requirements.txt
bash scripts/start_all.sh


