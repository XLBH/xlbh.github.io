# 3D 设计师作品集 / 3D Design Portfolio

朱碧航（Zhu Bihang）的 3D 设计师求职作品集，展示游戏道具资产制作、硬表面建模、PBR 材质与电商视觉渲染能力。

在线访问：GitHub Pages（见仓库 Settings → Pages）

## 作品内容

### Project 01 — 格洛克 19 手枪（写实道具 · 4K PBR 全流程）

- 以 Glock 19 Gen5 为原型的写实道具资产，Blender 硬表面建模 + Substance 3D Painter 绘制
- 规格：**2,610 顶点 / 2,369 面 / 4,764 三角面 / 20 个独立部件**
- **线框与 UV**：UV 分块排布 + 线框拓扑工作视图，单套 UV 覆盖全部部件
- **贴图集**：3 张 4096²（Base Color / Normal / ORM），ORM 按 R 遮蔽 · G 粗糙 · B 金属打包
- 4 张成品渲染：双枪俯视主视觉 + 双侧视细节图
- **UE5 实机验证**：资产导入引擎后在实时管线下的材质接入、比例与法线表现截图

### Project 02 — 蒸汽朋克手枪道具（游戏道具资产 · 高低模烘焙）

- **高低模同机位对比**：45° 大图对比 + 侧 / 正 / 背三机位，高模素模与低模烘焙成品并排验证
- **低模先行**：先搭低模定形与布线（**4,389 Tris**），再由同一模型细化出高模（**35,259 Tris**）作烘焙源，细节由 Normal 贴图承载还原
- 完整管线：Blender 低模建模 → 高模细化 → Substance 3D Painter 烘焙绘制（11 个 Texture Set）→ FBX 导入 3ds Max 重建 PBR 材质与灯光渲染

### Project 03 — S1 履带式防空车（复杂机械体 · UDIM 多分块管理）

- 4 张成品渲染：3/4 主视角 + 侧视 / 正视 / 俯视三视图
- **UV 布局**：UDIM 1001–1010 共 10 个图块总览 + 关键部件单独展开图（同心圆展开 · 接缝落在隐藏边）
- PBR 六通道拆解：Base Color、Normal、Roughness、Metallic、Height、AO

规格：247,758 三角面 / 31 个独立部件 / 171,087 条 UV 唯一边 / 10 个 UDIM 图块

### Project 04 — 电商产品视觉

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
assets/       35 张优化后的图片素材（渲染图 / UV 图 / 贴图集 / 引擎实机截图，约 4.6 MB）
```

---

Portfolio of Zhu Bihang — 3D Designer. Realistic game-ready props, high-to-low poly baking, hard-surface modeling, PBR texturing, and commercial product visualization.
