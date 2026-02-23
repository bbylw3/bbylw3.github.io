# 🌌 深空架构 // 神经元导航矩阵

_(BLACKWELL WEBNAV ARCHITECTURE)_

> 这是一个以极其硬核的工业级半导体美学，结合现代照片级 WebGL 渲染技术打造的“次世代 3D 浏览器主页导航”引擎。
> 本项目放弃了枯燥平庸的 2D 链接列表，而是将每一个目标网站的算力映射到了一颗完整复刻自 NVIDIA Blackwell 架构集群的光刻级芯片核心之上！

## 🚀 核心体验与功能特性 (Features)

- **PBR 照片级环境光照重塑**
  采用了 `RoomEnvironment` PMREM 加性渲染，完美复刻无暇的高纯度金属框架、超黑吸收基板、以及能够反射真实光源的工业玻璃质感表层，打破常规 Web3D 的虚假模型感。
- **深海级硅晶圆材质解析 (Procedural Micro-Silicon Texture)**
  纯通过数学着色器在 Canvas 端逐像素绘制出了 1024x2048 的微观 Tensor Core 硅胶排线结构纹理，并赋予了真实半导体出厂时的“Iridescence 彩虹干涉膜”炫彩光学反馈。
- **全息诊断态势感知 UI**
  完全移除低廉的浮动标签。悬停于任意硬件节点上，右侧暗色深框会自动滑出诊断面板，并带有一扫而过的神经接入“脉冲干扰 (Glitch)”。
- **沉浸式全局左栏映射 (Symmetrical UI-3D Sync)**
  为了兼顾纯粹导航体验，左侧悬浮有一排真正的毛玻璃导航矩阵框。**你可以像正常网站一样点击按钮跳转链接。当你滑过左侧 UI 时，右侧庞大的万兆芯片将通过高光爆闪来进行 1:1 双向物理反馈！**
- **高级全局中文化与专属定制字体**
  放弃了糟糕的系统备用黑体，全面引进了 `Noto Sans SC`（思源黑体）+ `JetBrains Mono`（极客等宽编码），字体字重与排版呈现顶级视觉团队出品水准。不再使用突兀的英语词汇，全面应用了形如“张量单元”、“主控核心”、“系统级就绪”等高概念中文语境。

## 🕹️ 接入节点矩阵 (Hardware Node Definitions)

| 系统 ID (System ID) | 宏模块节点代号 | 链接目的地                                      | 节点类型定义及带宽描述                                             | 色谱代号           |
| :------------------ | :------------- | :---------------------------------------------- | :----------------------------------------------------------------- | :----------------- |
| **00**              | NV-ROUTING     | [AVP 渲染空间](https://pornavp.onrender.com)    | 主控核心：接管并承载超高并发带宽媒体的纯硬解码流出                 | 青蓝 (`#00f0ff`)   |
| **01**              | COMPUTE_L      | [ChatGPT Core](https://chatgpt.com/)            | 张量单元：语言计算分片，负担着庞大文本流的嚼碎与深思推理           | 翠绿 (`#00ffaa`)   |
| **02**              | COMPUTE_R      | [Gemini Sub-System](https://gemini.google.com/) | 张量单元：多模态吞吐处理中心，用以抵御极度不稳定的音视网文电涌     | 紫罗兰 (`#cc00ff`) |
| **03**              | HBM3E_TOP      | [Google Matrix](https://www.google.com/)        | 高速显存：连接人类文明核心索引数据库的最高频外部金属插脚栈         | 玫红 (`#ff3366`)   |
| **04**              | HBM3E_BOT      | [Grok Unsanctioned](https://grok.com/)          | 混沌末端：卸除安全对齐机制，强行缓存来自全网不加修饰信号的特供显存 | 爆闪黄 (`#ffee00`) |

## ⚙️ 启动序列 (How to Launch)

这不再是一个简单的 HTML，它请求了巨量的本地贴图渲染与跨域的 `three.js` 解析，因此必须在本地服务器内运行。

1.  **Clone / Download** 整个该项目。
2.  在你电脑的终端里进入这个项目的根目录 `nav/StepFun`。
3.  唤醒你的本地 HTTP 服务器，最快的方法是运行 Python 3:
    ```bash
    python -m http.server 8000
    ```
4.  打开你最依赖并支持最新硬解的浏览器 (推荐 Edge / Chrome)。
5.  在地址栏输入：**`http://localhost:8000`**
6.  _(注意：千万不要使用包含 `[::]` 的 IPv6 地址进行开发调试，这会立刻遭到浏览器关于 `Three` 加包解析层的无情 CORS 残酷拦截！)_

## 🛠️ 技术基底 (Tech Stack)

- **Three.js (r170)**: 绝对引擎基石 (采用 PBR 标准工作流)。
- **CSS / UI**: Tailwind CSS 架接出的无断点原子类设计。
- **Fonts**: Google Fonts (`Inter` + `JetBrains Mono` + `Noto Sans SC`)。
- **Lighting Render**: `RoomEnvironment.js` (PMREMGenerator 构建极尽真实的高级泛光贴图烘焙体系)。
