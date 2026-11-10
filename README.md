## Dota2 Mini Game

基于 Python 和计算机视觉的 Dota 2 小游戏自动化实验项目。

## 项目简介

本项目旨在探索使用计算机视觉、运动预测和自动决策算法，实现 Dota 2「暗黑狂欢（Dark Carnival）」活动中小游戏的自动化分析与控制。

目前优先开发 **撬锁（Pick the Lock）** 小游戏，后续计划扩展至打砖块等其他小游戏。

## 技术栈

- **语言：** Python 3.12
- **包管理：** uv
- **图像处理：** OpenCV、NumPy
- **屏幕捕获：** Wayland 
- **输入控制：** pynput（兼容性待验证）
- **开发工具：** PyCharm、Pyrefly、Ruff、pytest
- **开发环境：** CachyOS + KDE Wayland

## 环境配置

克隆项目：

```bash
git clone <repository-url>
cd Dota2-mini-game
```

安装依赖：

```bash
uv sync
```

验证环境：

```bash
uv run python -c "import cv2, numpy, mss; print('Environment OK')"
```

## 开发计划

- [ ] 实现游戏画面捕获
- [ ] 识别撬锁指针和目标区域
- [ ] 计算指针角度及旋转速度
- [ ] 实现命中时机预测
- [ ] 实现可视化调试和离线测试
- [ ] 在独立测试环境中验证自动控制
- [ ] 扩展其他小游戏

## 项目状态

🚧 开发中（v0.1.0）

当前处于项目初始化阶段，尚未实现完整的小游戏识别与控制功能。

## 声明

本项目仅用于个人学习和技术研究，与 Valve 或 Dota 2 官方无关。使用第三方自动化工具操作正式游戏客户端可能违反 Steam 用户协议。