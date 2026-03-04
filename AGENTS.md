# AGENTS.md

## Cursor Cloud specific instructions

This repository (`browser-auto` — 浏览器自动化任务) is a browser automation project for Taobao tasks (e.g. 淘金币赚金币). The repo currently has no source code — it is a freshly initialized project with only a `README.md`.

### Current state

- **No source code, dependencies, or build system** — the repo has no application code yet.
- **No lint/test/build commands** configured.

### Browser automation environment

- Chrome browser is pre-installed and available for GUI-based automation via the `computerUse` subagent.
- Taobao login requires user interaction via the Desktop pane (QR code or phone number login).
- **Taobao anti-automation caveat**: Accessing product detail pages (`item.taobao.com`) from this cloud environment triggers Taobao's security system ("亲，访问被拒绝" / Access denied). Tasks that only require visiting activity pages (淘金币主页, 直播间, 购物车, 游戏中心) work fine. Product browsing tasks may fail due to this restriction.
- The 淘金币 page URL: `https://huodong.taobao.com/wow/z/tbhome/pc-growth/tao-coin`

### When code is added

Once source code and a dependency manifest are added to this repo, the update script and this file should be revised accordingly. Future agents should check for the presence of dependency files (`requirements.txt`, `pyproject.toml`, `package.json`, etc.) and install dependencies as needed.
