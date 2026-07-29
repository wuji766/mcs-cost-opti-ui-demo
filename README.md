# MCS 搬送监控系统 · UI Demo

纯前端静态演示，托管于 GitHub Pages。所有数据为 Mock 示例数据。

## 📺 页面

| 页面 | 说明 |
|---|---|
| [🏠 首页](index.html) | 入口导航 |
| [🔬 任务分析 & Cost 编辑](task-cost-merge.html) | 三模式驱动工作台：历史压力分析 / Cost 调整 / 调整仿真 |
| [🚀 Cost 上线管理](cost-apply.html) | 版本上线发布、上线记录、一键回退 |

## 🚀 本地预览

无需任何依赖，直接用浏览器打开 `index.html` 即可。或启动任意静态服务器：

```bash
python -m http.server 8080
# 访问 http://localhost:8080
```

## 🛠 技术栈

- 纯 HTML + CSS + 原生 JavaScript（无构建依赖）
- 内嵌 Mock 数据，演示交互逻辑
- 响应式布局，适配桌面浏览器

## 📁 结构

```
├── index.html              # 首页
├── task-cost-merge.html    # 任务分析 + Cost 编辑（三模式）
├── cost-apply.html         # Cost 上线管理（记录+回退）
├── real-viz.html           # 真实数据可视化（直方图均衡化+双向边）
└── assets/
    ├── app.css             # 共享样式
    ├── mcs_layout_min.svg  # 真实仓库布局 SVG（原项目同步）
    ├── real_edges.json     # 真实边数据（368边，来自 PG）
    └── real_layout.json    # 真实节点坐标（从 SVG 提取，252节点）
```

## ⚠️ 说明

本仓库仅包含 **UI 交互演示**，不含后端服务与真实数据。完整系统的前后端实现详见主项目。
