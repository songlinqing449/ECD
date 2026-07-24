# 🔬 电致变色器件 (ECD) — 交互式 3D 模型

> Electrochromic Device — Interactive 3D Model

一个基于 **Three.js** 的电致变色器件 (Electrochromic Device, ECD) 交互式 3D 模型。可以通过鼠标拖拽旋转、缩放，点击每一层查看详细介绍，适合用于教学演示、学术报告和科普展示。

## ✨ 功能特性

- **🖱 3D 交互** — 拖动旋转、滚轮缩放、右键平移
- **💥 分解/堆叠视图** — 一键切换展开或紧凑模式
- **⚡ 变色演示** — 动态展示电致变色层 (WO₃) 从透明到深蓝的可逆变色过程
- **📋 层详情面板** — 点击任意层或右侧图例查看详细材料、英文名称和工作原理
- **⌨ 键盘快捷键** — E/S/A/R/1-7/ESC 快速操作
- **🎨 现代 UI** — 暗色主题、粒子背景、动态光影
- **📱 响应式设计** — 适配桌面和移动端

## 🔬 器件结构 (7 层)

| 层号 | 名称 | 英文 | 典型材料 |
|------|------|------|----------|
| 1 | 玻璃基底（上） | Glass Substrate (Top) | 钠钙玻璃、PET |
| 2 | 透明导电层（上电极） | ITO (Top Electrode) | ITO、FTO |
| 3 | **电致变色层** | **Electrochromic Layer** | **WO₃、PEDOT:PSS** |
| 4 | 电解质/离子导体层 | Electrolyte Layer | LiClO₄/PC、LiPON |
| 5 | 离子存储层（对电极） | Ion Storage / Counter Electrode | NiO、CeO₂ |
| 6 | 透明导电层（下电极） | ITO (Bottom Electrode) | ITO、FTO |
| 7 | 玻璃基底（下） | Glass Substrate (Bottom) | 钠钙玻璃、PET |

## ⚙️ 工作原理

```
WO₃ (透明) + xLi⁺ + xe⁻  ⇌  LiₓWO₃ (深蓝色)
```

施加正向电压时，Li⁺ 离子从离子存储层穿过电解质注入 WO₃ 层，器件着色；
施加反向电压时，Li⁺ 离子迁回离子存储层，器件恢复透明。

## 🚀 使用方式

直接在浏览器中打开 `index.html` 即可，无需构建工具。

```bash
# 方式 1: 直接打开
open index.html

# 方式 2: 使用本地服务器 (推荐)
npx serve .
# 或
python -m http.server 8080
```

## ⌨ 快捷键

| 键 | 功能 |
|----|------|
| `E` | 分解视图 |
| `S` | 堆叠视图 |
| `A` | 变色演示 (开/关) |
| `R` | 重置视角 |
| `1-7` | 选择对应层 |
| `ESC` | 关闭详情面板 |

## 🛠 技术栈

- [Three.js](https://threejs.org/) — 3D 渲染引擎
- ES Modules (Import Map) — 模块加载
- 纯 HTML/CSS/JS — 零依赖、零构建

## 📄 License

MIT

---

🤖 Generated with [Claude Code](https://claude.com/claude-code)
