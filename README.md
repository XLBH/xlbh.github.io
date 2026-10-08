# 3D 设计师作品集 / 3D Design Portfolio

朱碧航（Zhu Bihang）的 3D 设计师求职作品集，展示游戏道具资产制作、硬表面建模、PBR 材质与电商视觉渲染能力。

在线访问：GitHub Pages（见仓库 Settings → Pages）

## 作品内容

### Project 01 — 蒸汽朋克手枪道具（游戏道具资产 · 高低模烘焙）

- **高低模同机位对比**：45° 大图对比 + 侧 / 正 / 背三机位，高模素模与低模烘焙成品并排验证
- 面数由高模 **35,259 Tris** 压至低模 **4,389 Tris**（保留 12.5%），细节由 Normal 贴图承载还原
- **贴图规范**：单张 1024² 贴图集覆盖 11 个 Texture Set，输出 D / N / MRA 三张贴图
- **MRA 三通道打包**：R 金属度 / G 粗糙度 / B 环境光遮蔽，附三通道拆分图
- 完整管线：Blender 高低模 → Substance 3D Painter 烘焙绘制 → 低模拓扑整理 → FBX 导入 3ds Max 重建 PBR 材质与灯光渲染

### Project 02 — S1 履带式防空车（复杂机械体 · UDIM 多分块管理）

- 5 张多视图渲染（侧视 / 正视 / 俯视 / 后视 / 三视角装配）
- **线框 / 拓扑验证**：整车 3/4 与侧视线框、行走机构 / 车首 / 传动轮 / 武器系统 4 张局部特写
- **UV 布局**：UDIM 1001–1010 共 10 个图块总览 + 关键部件单独展开图（同心圆展开 · 接缝落在隐藏边）
- PBR 六通道拆解：Base Color、Normal、Roughness、Metallic、Height、AO

规格：247,758 三角面 / 31 个独立部件 / 171,087 条 UV 唯一边 / 10 个 UDIM 图块

### Project 03 — 电商产品视觉

- 儿童学习桌椅组合、户外藤编旋转椅
- 涵盖场景搭建、布光渲染、色彩构成与材质表现

## 技术栈

Blender · Substance 3D Painter · 3ds Max · Unreal Engine 5 · Unity · Marvelous Designer · Photoshop · Premiere Pro

## 本地运行

纯静态站点，零构建依赖。直接打开 `index.html` 即可，或起一个本地服务：

```bash
python3 -m http.server 8000
```

## 目录结构

```
index.html    单文件页面（含全部样式与脚本）
assets/       39 张优化后的图片素材（渲染图 / 高低模对比 / 贴图集 / 线框图 / UV 图，约 7 MB）
```

---

Portfolio of Zhu Bihang — 3D Designer. Game-ready prop assets, high-to-low poly baking, hard-surface modeling, PBR texturing, and commercial product visualization.
