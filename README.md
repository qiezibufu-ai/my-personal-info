# 刘锦桉 · 个人主页与工程作品集 (Personal Portfolio)

> **广东工业大学 · 集成电路学院 · 2026级集成电路1班**  
> 专注于嵌入式系统、无刷电机 FOC 矢量控制、4 层硬件 PCB 设计与端侧边缘智能计算。

---

## ⚡ 架构亮点：极致“物理级秒开”

本项目遵循极客级性能优化指标与现代语义化 Web 标准开发，实测首屏渲染性能指标：

* **单包即达（Single Packet Delivery）**：Gzip 传输体积仅 **~9 KB**，严格控制在 TCP 初始拥塞窗口（`initcwnd ≈ 14 KB`）之内，**1 次 RTT 即可完成全站资源下载**。
* **0 外部阻塞资源**：
  * **0 外部 CSS 文件**：样式高度整合并直接内联在 `<head>`，无任何样式白屏阻塞。
  * **0 外部 JavaScript 运行时**：无 React/Vue 庞大框架负担，无 DOM 水合（Hydration）消耗，主线程瞬时绘制。
  * **0 外部图片请求**：芯片微架构图、电路走线纹理、系统图标全采用**原生内联 SVG** 渲染。
  * **0 外部字体包请求**：采用操作系统原生字体族（PingFang SC, Microsoft YaHei, -apple-system），杜绝字体闪烁（FOIT/FOUT）。
* **多端响应式与暗色模式**：完美适配桌面端、平板与手机屏幕，并支持系统深色模式（Dark Mode）。

---

## 📂 项目结构

```plaintext
my-personal-info/
├── index.html                           # 核心秒开主页 (单包即达, 纯语义化HTML5+内联CSS+矢量SVG)
├── snake.html                           # 芯片寻迹 · 3D 贪吃蛇交互体验 (集成电路主题 3D 游戏)
├── output/
│   └── pdf/
│       └── 刘锦桉_个人简介_详细版.pdf      # 完整个人简历 PDF (支持一键离线与在线下载)
└── README.md                            # 项目与部署说明文档
```

---

## 🚀 本地预览

直接在任意现代浏览器（Chrome、Edge、Safari、Firefox）双击打开 `index.html` 即可极速体验：

```bash
# 或者使用 Python 快速起一个轻量本地测试服务
python -m http.server 8080
# 访问 http://localhost:8080 即可
```

---

## 🌐 部署至 GitHub Pages（全免费 + 全球 CDN 加速）

1. **推送代码至 GitHub 仓库**：
   ```bash
   git init
   git add .
   git commit -m "feat: release instant-loading personal portfolio"
   git branch -M main
   git remote add origin https://github.com/qiezibufu-ai/my-personal-info.git
   git push -u origin main
   ```

2. **一键开启 GitHub Pages**：
   - 登录 GitHub，进入仓库页面：[`qiezibufu-ai/my-personal-info`](https://github.com/qiezibufu-ai/my-personal-info)
   - 点击顶部 **Settings** -> 左侧菜单 **Pages**
   - 在 **Build and deployment** 下：
     - **Source**: `Deploy from a branch`
     - **Branch**: `main` / `/(root)`
     - 点击 **Save**
   - 等待约 1 分钟，GitHub Pages 即可自动完成构建，获得专属访问网址：
     👉 `https://qiezibufu-ai.github.io/my-personal-info/`

---

## 📬 联系方式

* **Email**: 615873738@qq.com
* **Phone**: 18998364503
* **QQ / WeChat**: 615873738
* **GitHub**: [@qiezibufu-ai](https://github.com/qiezibufu-ai)
