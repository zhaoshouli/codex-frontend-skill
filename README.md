# Codex 前端实现 Skill

这是一个可复用的 Codex skill，用于实现前端应用、页面和交互式工具，并配套实际可执行的构建与浏览器验收流程。

## Skill

- `frontend-implementation`：当 Codex 需要构建、修改或打磨网页前端时使用，包括 React/Vite 应用、静态 HTML/CSS/JS 页面、仪表盘、表单和浏览器工具。

## 安装

把 skill 文件夹复制到你的 Codex skills 目录：

```bash
mkdir -p ~/.codex/skills
cp -R skills/frontend-implementation ~/.codex/skills/
```

安装后重启 Codex，让它发现新的 skill。

## 使用

可以显式要求 Codex 使用这个 skill：

```text
使用 $frontend-implementation 构建这个仪表盘页面，并在浏览器里验证。
```

当任务匹配 skill 描述时，Codex 也可以自动调用它。
