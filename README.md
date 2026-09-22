# 3D 设计师作品集 / 3D Design Portfolio

朱碧航（Zhu Bihang）的 3D 设计师求职作品集，展示硬表面建模、PBR 材质制作与电商视觉渲染能力。

在线访问：GitHub Pages（见仓库 Settings → Pages）

## 作品内容

### Project 01 — S1 履带式防空车（硬表面建模）

- 5 张多视图渲染（侧视 / 正视 / 俯视 / 后视 / 三视角装配）
- PBR 六通道拆解：Base Color、Normal、Roughness、Metallic、Height、AO
- 9 组分件贴图集（UDIM 多分块，4K / 2K / 1K 分级）
- 完整制作流程：Blender 建模 → UV/UDIM 拆分 → Substance 3D Painter 烘焙绘制 → 贴图回接 → 渲染输出

### Project 02 — 电商产品视觉

- 儿童学习桌椅组合、户外藤编旋转椅
- 涵盖场景搭建、布光渲染、色彩构成与材质表现

## 技术栈

Blender · Substance 3D Painter · Unreal Engine 5 · Unity · Marvelous Designer · Photoshop · Premiere Pro

## 本地运行

纯静态站点，零构建依赖。直接打开 `index.html` 即可，或起一个本地服务：

```bash
python3 -m http.server 8000
```

## 目录结构

```
index.html    单文件页面（含全部样式与脚本）
assets/       22 张优化后的图片素材（约 2 MB）
```

---

Portfolio of Zhu Bihang — 3D Designer. Hard-surface modeling, PBR texturing, and commercial product visualization.
