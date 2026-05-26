# 🤝 协作开发指南

欢迎加入持仓同步项目的开发！本指南将帮助你快速上手。

## 📋 目录
- [快速开始](#快速开始)
- [开发流程](#开发流程)
- [代码规范](#代码规范)
- [提交规范](#提交规范)
- [联系方式](#联系方式)

## 🚀 快速开始

### 1. Fork 和 Clone 仓库
```bash
# Clone 主仓库
git clone https://github.com/bosco666/-.git
cd -

# 添加上游仓库
git remote add upstream https://github.com/bosco666/-.git
```

### 2. 创建开发分支
```bash
# 从 develop 分支创建你的开发分支
git checkout -b feature/your-feature-name develop

# 或者创建修复分支
git checkout -b bugfix/your-bug-name develop
```

### 3. 进行开发
- 在你的分支上开发新功能或修复问题
- 定期提交代码，使用有意义的提交信息

## 📝 开发流程

### 分支命名规范
- **功能分支**: `feature/功能描述` (例如: `feature/add-sync-engine`)
- **修复分支**: `bugfix/问题描述` (例如: `bugfix/fix-data-loss`)
- **文档分支**: `docs/文档描述` (例如: `docs/update-readme`)
- **测试分支**: `test/测试描述` (例如: `test/add-unit-tests`)

### 提交流程
```
1. 在你的分支上完成开发
2. 提交代码到远程分支
3. 在 GitHub 上创建 Pull Request (PR)
4. 等待代码审查
5. 根据反馈进行调整
6. 合并到主分支
```

## 💻 代码规范

### Python 代码规范
- 遵循 PEP 8 规范
- 使用有意义的变量名和函数名
- 添加必要的注释和文档字符串
- 确保代码可读性和可维护性

### 提交信息规范
采用以下格式：
```
<type>(<scope>): <subject>

<body>

<footer>
```

**Type 类型**:
- `feat`: 新功能
- `fix`: 错误修复
- `docs`: 文档更新
- `style`: 代码格式（不影响代码逻辑）
- `refactor`: 代码重构
- `perf`: 性能优化
- `test`: 添加测试
- `chore`: 构建配置或依赖更新

**例子**:
```
feat(sync): 添加实时数据同步功能

添加了基于 WebSocket 的实时数据同步机制，
支持多用户并发更新持仓数据。

Closes #123
```

## 🔄 完整工作流示例

```bash
# 1. 更新本地 main 分支
git checkout main
git pull upstream main

# 2. 创建开发分支
git checkout -b feature/new-feature main

# 3. 进行开发和提交
git add .
git commit -m "feat(component): 添加新功能"

# 4. 推送到远程
git push origin feature/new-feature

# 5. 在 GitHub 上创建 PR
# 访问 https://github.com/bosco666/-
# 点击 "New Pull Request" 按钮

# 6. 等待审查和合并
```

## ✅ PR 检查清单

提交 PR 前，请确保：
- [ ] 代码遵循项目的代码规范
- [ ] 提交信息清晰有意义
- [ ] 添加了相关的测试（如果适用）
- [ ] 更新了文档（如果适用）
- [ ] 没有未解决的冲突
- [ ] 通过了所有 CI 检查

## 📞 联系方式

- 📧 Email: bosco666@example.com
- 💬 Discussions: GitHub Discussions
- 🐛 Issues: GitHub Issues

## 📄 许可证

本项目采用 MIT 许可证。详见 [LICENSE](LICENSE) 文件。

---

感谢你的贡献！👏
