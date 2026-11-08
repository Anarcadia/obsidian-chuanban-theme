# chuanban — Warm Editorial & Long-Form Writing Theme for Obsidian

![chuanban Theme Screenshot](screenshot.png)

**chuanban** is a warm, high-contrast paper-and-ink light theme crafted for novelists, essayists, and deep long-form writers in Obsidian. It combines warm ivory and oat paper surfaces, terracotta accents, tactile ink-softening typography, and high-density page preview popovers.

---

## ✨ Key Features / 核心特性

### 1. Warm Ivory & Oat Editorial Palette (暖白象牙与燕麦纸感色彩体系)
- **Primary Reading Canvas (`#FCFCFB`)**: Micro-warm ivory paper surface that eliminates cold digital glare (`#FFFFFF`) while keeping crisp text contrast (`#1F1E1D`).
- **Sidebar & Navigation (`#F7F5F0`)**: Warm oat secondary background with deep oat active pills (`#ECE9E1`) and crisp `1px` dividers (`rgba(0, 0, 0, 0.14)`).
- **Terracotta Accent (`#D97757`)**: Used for active tabs, blockquotes, links, and focus indicators.
- **Eye-Care Selection & Highlight**: Soft sage-green text selection (`rgba(130, 175, 138, 0.24)`) + warm amber marker highlight (`rgba(232, 197, 110, 0.28)`).

### 2. Built-in CJK/Western Typography Styles (内置双排版样式)
> **Note**: As an official Obsidian Community Theme, this package is a **pure CSS theme** and does not bundle any third-party plugins. Out of the box, it defaults to **Typewriter Slab**. If you wish to switch to the built-in **Classic Songti Serif** style, you can either add `cssclasses: [preset-songti-serif]` to a note's YAML frontmatter or use the community **Style Settings** plugin (`chuanban -> Typography Preset`).

| Feature | Default: Typewriter Slab (更纱打字机体 · 默认开箱即用) | Optional: Classic Songti Serif (经典书卷宋体 · `preset-songti-serif`) |
| :--- | :--- | :--- |
| **Font Stack** | `Sarasa Mono Slab SC` (`等距更纱黑体 Slab SC`) | Western Sans (`SF Pro Text` / `Inter`) + `Songti SC` (`宋体-简` 全角方块排布) |
| **Line Height** | `1.78` | `1.68` |
| **Paragraph Gap** | `0.38em` (Live Preview) / `0.95em` (Reading) | `0.82em` (Live Preview) / `1.05em` (Reading) |
| **Ink Texture** | `0.25px` subtle ink-bleed softening | Crisp, un-shadowed serif strokes + `tabular-nums` & `full-width` CJK |

### 3. Decoupled High-Density Page Preview Popover (固定高信息量悬浮预览卡)
- Page preview popovers (`.popover.hover-popover`) are decoupled from the main editor's zoom level and locked at a crisp **`13px` / `1.52` line-height** (`440×360px` scrollable viewport).
- Automatically hides YAML frontmatter properties (`.metadata-container`) inside hover previews so you immediately see the body text.

---

## 🔤 Recommended Fonts / 推荐字体安装

For the best typography experience on macOS / Windows / Linux:
1. **Sarasa Mono Slab SC (`等距更纱黑体 Slab SC`)** — Recommended for the default Typewriter Slab style:
   ```bash
   brew install --cask font-sarasa-gothic
   ```
2. **Songti SC (`宋体-简`)** — Built into macOS for the optional Classic Songti Serif style.

---

## 📝 Changelog / 更新日志

See [CHANGELOG.md](CHANGELOG.md) for full details.

- **`v1.0.3` (2026-11-08)** — **Windows / Linux / macOS Hidden Frameless Titlebar Compatibility Fix (Windows/Linux 隐藏标题栏模式顶栏遮挡与窗口按钮预留区修复)**:
  - Fixed `.titlebar` forcing an opaque background in `body.is-hidden-frameless` mode on Windows/Linux, which previously covered the top-left and top-right sidebar icons and tab bar.
  - Preserved `--frame-left-space` and `--frame-right-space` on `.workspace-tabs.mod-top-left-space` / `.mod-top-right-space` so top-right icons never collide with Windows `- □ ×` window buttons or macOS traffic lights.
  - Added `.mod-right-split .workspace-tab-header-inner` and `.workspace-tab-header-container-inner` resets to prevent right-sidebar icon clipping.
- **`v1.0.2` (2026-11-02)** — Updated theme showcase screenshot and clarified built-in typography presets (`preset-songti-serif`).
- **`v1.0.1` (2026-11-02)** — Standardized typography stacks on open-source (`Sarasa Mono Slab SC`, `Inter`, `JetBrains Mono`) and native system fonts.
- **`v1.0.0` (2026-11-01)** — Initial official release of `chuanban`.

---

## 📄 License

[MIT License](LICENSE) © 2026 chuanban ([Anarcadia](https://github.com/Anarcadia))
