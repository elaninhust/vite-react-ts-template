## vite-react-ts-template

这是基本 Vite 官方提供的模板改造的适合快速新建项目的优化后的项目模板。

> 原官方模板地址：[@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md)

增加的功能如下：

**main** 分支

- [x] eslint
- [x] prettier
- [x] husky
- [x] lint-staged
- [ ] commitlint
- [ ] commitizen

**eslint-tailwindcss** 分支

使用 `eslint-plugin-tailwindcss` 来检查 `tailwindcss`

- [x] eslint
- [x] prettier
- [x] husky
- [x] lint-staged
- [x] tailwindcss
- [ ] commitlint
- [ ] commitizen

**prettier-tailwindcss** 分支

使用官方推出的 `prettier-plugin-tailwindcss` 来检查 `tailwindcss`

- [x] eslint
- [x] prettier
- [x] husky
- [x] lint-staged
- [x] tailwindcss
- [ ] commitlint
- [ ] commitizen

**chrome-extension** 分支

参考 [chrome-extension-boilerplate-react-vite](https://github.com/Jonghakseo/chrome-extension-boilerplate-react-vite) 仓库搭建的快速开发 `chrome-extension` 的结构

- [x] eslint
- [x] prettier
- [x] husky
- [x] lint-staged
- [ ] tailwindcss
- [ ] commitlint
- [ ] commitizen
- [x] manifest.config.ts

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:

- Configure the top-level `parserOptions` property like this:

```js
   parserOptions: {
    ecmaVersion: 'latest',
    sourceType: 'module',
    project: ['./tsconfig.json', './tsconfig.node.json'],
    tsconfigRootDir: __dirname,
   },
```

- Replace `plugin:@typescript-eslint/recommended` to `plugin:@typescript-eslint/recommended-type-checked` or `plugin:@typescript-eslint/strict-type-checked`
- Optionally add `plugin:@typescript-eslint/stylistic-type-checked`
