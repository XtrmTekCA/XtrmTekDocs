# Github 提交规范

---

### Commit message 格式

```
<type>(<scope>): <subject>
// 注意冒号 : 后有空格
// 如 feat(Device): Added device configuration UI
```

### 常用 types：

- feat (添加新特性, 包括 UI 样式的更新)
- fix (修复 bug)
- docs (修改文档)
- style (修改了代码格式，逗号，空格等，不改变代码逻辑以及 UI 样式)
- refactor (代码重构，没有添加新功能或者修复 bug)
- perf (代码优化，提升性能，体验)
- test (添加测试用例)
- build (修改打包文件相关内容)
- ci (修改配置相关文件，如 docker-compose.yml 文件)
- chore (辅助工具的变动或依赖包的变动， 如 node_modules)

> **注：** 推荐使用 VSCode 中的 [git-commit-plugin](https://marketplace.visualstudio.com/items?itemName=redjue.git-commit-plugin) 插件来简化操作和学习成本
