## 🌟 项目概览 (Project Overview)

本项目包含多种风格各异的实验页面，通过双击相应的 HTML 文件即可在浏览器中预览：

### 1. 🖐️ 手势与计算机视觉交互 (Hand & Pose Tracking)
- **`index.html`** - **分形万花筒 (Fractal Kaleidoscope - Debug Panel)**
  使用 ML5.js 的手部关键点追踪。支持识别多种手势（张开、捏合、旋转），通过手势距离、角度和捏合状态来实时控制动态分形着色器（Shader）。内置中英双语调试面板。
- **`color2.html`** - **分形万花筒 — 手势魔法**
  与 `index.html` 核心类似，侧重于展现绚丽的分形图像，通过手部动作实时施展视觉魔法。
- **`color.html`** - **手部交互着色器**
  一个基础的 WebGL Shader 交互实验，通过捕捉手部在屏幕空间的位置来改变色彩和流体形态。
- **`sensor.html`** - **Three.js + MediaPipe Holistic**
  结合了强大的 MediaPipe Holistic（人体、面部、手势综合追踪）与 3D 渲染引擎 Three.js。通过肢体动作驱动 3D 场景中的对象。
- **`Tina.html`** - **Tracking Test Interface**
  用于追踪算法测试和阈值校准的接口界面。

### 2. 🪄 生成艺术与特效处理 (Generative & Effect)
- **`Moodboard.html`** - **AI Moodboard (智能灵感板)**
  一个集成了拖拽、排列、自动化布局等功能的创意板（Moodboard）应用，用于艺术家收集和整理视觉灵感。
- **`oil.html`** - **印象派油画生成器**
  上传或拖拽图片，算法会通过随机笔触、噪声和颜色采样，在 Canvas 上自动将普通图像转换为具有笔触质感的印象派油画效果。

### 3. 🎐 物理模拟与 3D (Physics & 3D)
- **`kite.html`** - **3D 交互风筝**
  使用 3D 图形技术模拟风筝的动态与风力交互，支持拖拽和视角的变换。
- **`Cupid.html`** - **Cupid's Arrow - AI Interactive**
  结合互动特性的射箭/丘比特主题互动游戏，可能有鼠标或姿态追踪进行目标判定。

---

## 🚀 运行方式 (How to Run)

**环境要求极低，开箱即用：**

1. 推荐使用现代浏览器（如 **Google Chrome**, **Edge** 或 **Safari**）。
2. 在文件管理器中，直接 **双击相应的 HTML 文件** 即可在浏览器中运行。
3. **摄像头权限：** 对于依赖 `ml5.js` 或 `MediaPipe` 的项目（如 `index.html`, `color.html`, `sensor.html` 等），浏览器会请求摄像头权限，请点击 **允许 (Allow)**。如果无法获取摄像头，画面或交互可能会失效。
4. **提示：** 某些本地安全策略可能会限制摄像头的访问（`file://` 协议下）。如果出现问题，建议使用简单的本地服务器（例如 VS Code 的 Live Server 插件，或在终端中运行 `python -m http.server 8000`）并在 `http://localhost:8000` 中打开。

---

## 🛠️ 技术栈 (Technologies Used)

* **[p5.js](https://p5js.org/)** / **[ml5.js](https://ml5js.org/)**: 快速进行创意编程与在浏览器中运行轻量级机器学习模型（手部识别等）。
* **[Three.js](https://threejs.org/)**: 强大的 WebGL 3D 渲染引擎。
* **[MediaPipe](https://mediapipe.dev/)**: Google 开源的跨平台机器学习感知流水线，用于高精度的人体（Holistic/Hand）追踪。
* **WebGL & GLSL Shaders**: 运行在 GPU 上的高阶片元着色器，用于渲染复杂的分形和光影效果。
* **HTML5 Canvas / SVG API**: 用于图像处理、半调效果或油画生成。

---

*“在代码的严谨与算法的偶然性中，寻找属于机器时代的艺术。”*
