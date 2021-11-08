# 代码格式规范

下载 VSCode 中的 [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) 插件来进行自动规范

> **⚠️ 注意<br />
> Prettier 仅能自动处理代码格式方面的规范问题，并不能自动处理语法及命名方面的错误，在编程过程中，请不要过度依赖 Prettier， 请自觉遵守驼峰命名格式，并在变量命名时要注意起有意义的名字**

```.prettierrc.js
module.exports = {
  bracketSpacing: true,
  jsxBracketSameLine: true,
  singleQuote: true,
  trailingComma: 'all',
  arrowParens: 'avoid',
};

```
