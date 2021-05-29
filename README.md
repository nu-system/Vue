# @\_nu/vue

💪 一个无 UI 依赖的 Vue 母版组件库系统

## Feature

- lerna: 用 lerna 来处理发布问题
- yarn workspace: 用 yarn 来处理依赖问题
- nwb: 用 nwb 处理 react demo 问题
- father: 做 React 组件构建
- gulp: 做 CSS 组件构建

## 开发 npm-scripts

```bash
$ lerna list  # 查看组件列表
$ yarn build // 构建
$ yarn cz    // 代码提交
$ lerna publish // 发布代码
```

## 开发 workspace

```html
$ yarn workspace @_nu/vue-button # 初始化，首次使用需要执行
$ yarn dev:*                     # 开发（ 需要在 npm-scripts 配置 ）
$ yarn build:*                   # 构建（ 需要在 npm-scripts 配置 ）
$ yarn workspace @_nu/vue-button add package           // 为组件添加依赖
$ yarn workspace @_nu/vue-button add package -W        // 默认添加添加依赖
$ yarn workspace @_nu/vue-button jest // 跑测试
```

