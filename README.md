# Neural Chip X1 - AI 导航网站

一个基于 Three.js 的高度仿真 AI 芯片可视化导航网站。

## 功能特性

### 3D 可视化
- 高度仿真的 AI 芯片模型
- PCB 基板 + 走线 + 电容
- 金色核心 DIE + 电路网格
- 散热顶盖 (IHS)
- 散热器 + 热管
- 镀金引脚

### 交互功能
- **Auto Rotate** - 自动旋转展示
- **Explode View** - 爆炸分解视图
- **Data Flow** - 数据流粒子动画
- **Wireframe** - 线框模式
- **Reset** - 重置视角

### 导航链接
- 🧭 AI Navigator - AI 工具导航平台
- 💬 ChatGPT - OpenAI 对话助手
- ✨ Gemini - Google 多模态 AI
- 🔍 Google - 全球搜索引擎
- 🚀 Grok - xAI 智能助手

## 技术栈

- **Three.js** - 3D 渲染引擎
- **ES Modules** - 现代 JavaScript 模块
- **OrbitControls** - 轨道控制器
- **WebGLRenderer** - WebGL 渲染器

## 本地运行

直接在浏览器中打开 `index.html` 文件即可运行。

或使用本地服务器：

```bash
# 使用 Python
python -m http.server 8080

# 使用 Node.js
npx serve
```

然后访问 `http://localhost:8080`

## 文件结构

```
StepFun/
├── index.html    # 主页面（包含 HTML、CSS、JS）
└── README.md     # 项目说明
```

## 配色方案

| 用途 | 颜色代码 |
|------|----------|
| 背景 | `#08080c` |
| 金色强调 | `#e8c47c` |
| 芯片基底 | `#1c1c1e` |
| 核心金色 | `#c9a045` |
| PCB 绿色 | `#0d2818` |
| 铜色热管 | `#b87333` |
| 镀金引脚 | `#d4af37` |
| 银色散热 | `#a8a8a8` |

## 浏览器支持

- Chrome (推荐)
- Firefox
- Safari
- Edge

需要支持 WebGL 和 ES Modules 的现代浏览器。

## 许可证

MIT License
