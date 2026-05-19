# Cursor 开发规范

本仓库在 Cursor 中协作时的约定，供人与 AI 共用。

## 项目约定

- **语言**：Node.js（无额外框架），入口为 `index.js`
- **运行**：`npm start` 或 `node index.js`
- **改动范围**：保持小步、可验证；不引入未说明的第三方依赖

## 与 AI 协作

1. **先读再改**：改代码前先看 `index.js`、`package.json` 和已有规则
2. **小步提交**：一次只做一件事，提交信息写清「为什么」
3. **不猜需求**：需求不清时先问，不擅自加功能或重构
4. **测试**：改完后用 `npm start` 确认能跑通

## 代码风格

- 使用项目已有风格，不混用多种格式
- 函数职责单一，避免深层嵌套
- 注释只写非显而易见的设计或业务逻辑
- 变量与文件名语义清晰（英文命名）

## Git

- 分支：`main` 为主分支
- 提交信息：简短中文或英文均可，说明改动目的
- 勿提交：`node_modules/`、`.env`、密钥与本地配置

## Cursor Rules

持久化规则放在 `.cursor/rules/`，Agent 会自动加载。详见该目录下的 `.mdc` 文件。

## 常用命令

```bash
npm start          # 运行 Hello World
git status         # 查看变更
git add . && git commit -m "说明"   # 提交（需自行 push）
```
