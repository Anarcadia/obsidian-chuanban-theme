# Changelog / 更新日志

All notable changes to **`chuanban`** are documented in this file.

---

## [1.0.3] - 2026-11-08

### Fixed / 修复
- **Windows / Linux Hidden Frameless `.titlebar` Overlay Fix（修复 Windows/Linux 隐藏标题栏模式下 `.titlebar` 不透明背景遮挡整个顶栏图标）**:
  - Scoped opaque `.titlebar` background & bottom border to `body:not(.is-hidden-frameless) .titlebar`, and explicitly enforced `background: transparent !important; border: none !important; pointer-events: none !important; height: calc(var(--header-height) - 1px) !important` on `body.is-hidden-frameless:not(.starter, .is-popout-modal) .titlebar`.
- **Window Control Safe Space `--frame-left-space` & `--frame-right-space` Preservation（恢复 Windows 右上角 `- □ ×` 窗口按钮与 macOS 红绿灯安全预留区）**:
  - Replaced hardcoded horizontal `padding` on `.workspace-tab-header-container` with explicit `.mod-top-left-space` / `.mod-top-right-space` padding formulas (`calc(10px + var(--frame-right-space, 0px))` on Windows/Linux, `calc(38px + var(--frame-right-space, 0px))` on macOS).
- **Right Sidebar Icon Inner Padding Reset（消除右侧栏小图标内部 `padding: 0 6px` 挤压裁切）**:
  - Added `.mod-right-split .workspace-tab-header-inner` and `.workspace-tab-header-container-inner` resets so right-sidebar `28×28px` icon buttons center cleanly without clipping.

---

## [1.0.2] - 2026-11-02

### Changed / 变更
- Updated theme demonstration screenshot, clarified pure-CSS typography preset options (Style Settings / `cssclasses`), and renamed Classic Songti Serif preset (`preset-songti-serif`, backward-compatible).

---

## [1.0.1] - 2026-11-02

### Changed / 变更
- Standardized typography stacks on 100% open-source (`Sarasa Mono Slab SC`, `Inter`, `DM Sans`, `JetBrains Mono`, `Source Serif 4`, `Newsreader`) and native system fonts (`SF Pro Text`, `Songti SC`).

---

## [1.0.0] - 2026-11-01

### Added / 新增
- Initial official release of **`chuanban` — Warm Editorial & Long-Form Writing Theme for Obsidian**.
