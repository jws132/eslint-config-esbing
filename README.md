## ESLint 规范

个人前端 ESLint 规范，目前支持`vue|react`

#### 安装

```shell
npm install @jzo/eslint-config-esbing -D
# OR
yarn add @jzo/eslint-config-esbing --dev
```

#### 使用

在你的工程根目录下创建一个`.eslintrc.js`配置文件

配置如下:

- **基础配置**

```js
module.exports = {
  extends: ['@jzo/esbing']
}
```

- **vue**

```js
module.exports = {
  extends: ['@jzo/esbing/vue']
}
```

- **react**

```js
module.exports = {
  extends: ['@jzo/esbing/react']
}
```

:::caution
如果项目之前安装过 ESLint 相关的包，建议卸载，避免引入不必要的包。如`eslint`、`eslint-plugin-vue`、`@babel/eslint-parser`、`@typescript-eslint/eslint-plugin` 、`@typescript-eslint/parser`、`@vue/eslint-config-typescript`、`eslint-config-react-app`、
`eslint-plugin-import`等，直接在 package.json 搜索**eslint**，相关的包全部卸载
:::

版本更新

```
0.0.3 更新react/jsx-curly-spacing 配置
```
