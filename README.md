# THE MONOLITH // WebNav Hub

<div align="center">
  <h3>基于 WebGPU + Three.js TSL 驱动的次世代全连接科幻导航矩阵</h3>
</div>

---

## 🔮 核心概念 (Core Concept)

This is not a traditional website. 这是一个展现浏览器图形学前沿能力的极限测试场。基于最纯净的 `HTML` 骨架，通过原生 ES Modules 引入 `Three.js (r170)` 引擎引擎，并全面启用在浏览器端尚属前沿的 **WebGPU** 加速能力以及 **TSL (Three.js Shading Language)**。

它创造了一个巨大的悬浮数字几何单体（The Monolith），当用户在极具赛博格视觉质感（Anti-Slop 美学，拒绝平庸的大圆角和硅谷明亮风）的 UI 菜单间穿梭时，整个节点矩阵也会响应光标位置及导航属性产生空间物理扭曲和高阶的形态变异。

## 🚀 技术栈特性 (Tech Stack & Features)

**0 Dependencies Build System**
未采用任何如 React, Vue 等重量级框架。全程依赖轻量化的 HTML + ES Import Map 和 Tailwind CSS，提供最快的加载速度与最高自由度的底层 Shader 渲染控制。

### 核心亮点：

1. **百万实体级 GPGPU 粒子并发与网格实例**
   全面利用 WebGPU 的渲染管线，实现了由 8000 个 `CylinderGeometry` 单体组成的实例化球体。所有几何体的物理位置、旋转并非由 CPU 进行循环绘制，而是交由 GPU 处理。
2. **纯原生 TSL (NodeMaterial)着色器系统**
   彻底抛弃老旧的 `GLSL` 纯文件字符串编写模式。运用 TSL（节点化着色器语法），使用诸如 `positionLocal`, `time`, `instanceIndex` 动态化操纵各个切片模型。完美融合了基于材质的光照、环境遮蔽与次表面发光 (`MeshStandardNodeMaterial`)。
3. **量子流体力学响应与避让（Cursor Repulsion Field）**
   当鼠标在屏幕空间滑动时，系统会将 `Mouse Vector2` 实时反投影回真实的 `Vector3` 的世界切面。并由着色器内部在 GPU 上计算全域几何体与该投影点的欧氏距离差，极短时间内生成负向张力弹开晶体群（模拟引力避让效应）。
4. **状态机的物理相位映射 (Phase Morphing)**
   每一次 UI 层面的悬停，不仅调度 `DOM` 级卡片渲染，还在同一 tick 将状态机的目标 Uniforms 透传至 `WebGPU Engine`，驱动 `8000` 个节点发生从球形约束、向外膨胀到完全量子打散溃缩的变化周期。

---

## 🧭 WebNav Hub 节点网络 (Nodes)

当前系统包含 5 个关键数字边界网关：

| 节点代码 | 系统定义            | 导航枢纽层向对应域                                        |
| :------- | :------------------ | :-------------------------------------------------------- |
| `01`     | **WebNav Hub**      | [AVP 渲染空间 / 流媒体母舰](https://pornavp.onrender.com) |
| `02`     | **Google 核心搜索** | [全知搜索网络](https://www.google.com/)                   |
| `03`     | **ChatGPT**         | [第一代生成式语言模型核心](https://chatgpt.com/)          |
| `04`     | **Google Gemini**   | [多模态张量智能网格](https://gemini.google.com/)          |
| `05`     | **Grok 神经网络**   | [高频无约束宇宙级神经网络提纯器](https://grok.com/)       |

---

## 🛠️ 启动说明 (Initialization)

由于项目采用了极其前沿的 `Three.js` CDN `ES Modules` 原生引入机制，您无法直接通过双击 `index.html` 游玩（浏览器跨域安全策略会阻止 Import Map）。

**你需要通过任何简单的 HTTP 服务器容器进行启动。**

### 方法 1: 使用 Python (如果你有 Python 环境)

1. 打开终端输入：

```bash
python -m http.server
```

2. 在浏览器中打开：`http://localhost:8000`

### 方法 2: 使用 Node.js / NPM

1. 通过 `npx` 启动临时的 serve 服务：

```bash
npx serve
```

2. 在浏览器中打开：`http://localhost:3000`

_(注：系统必须依赖支持 WebGPU 特性的现代浏览器内核，如 Chrome 113+ 或者 Edge 113+。不支持的情况将会由底层回退至 WebGL Fallback)_

---

<div align="center">
  <strong>"The boundaries of imagination are computationally defined."</strong>
</div>
