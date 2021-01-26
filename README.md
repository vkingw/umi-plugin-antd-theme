<!-- @format -->

# umi-plugin-antd-theme-ng

[![NPM version](https://img.shields.io/npm/v/umi-plugin-antd-theme-ng.svg?style=flat)](https://npmjs.org/package/umi-plugin-antd-theme-ng) [![NPM downloads](http://img.shields.io/npm/dm/umi-plugin-antd-theme-ng.svg?style=flat)](https://npmjs.org/package/umi-plugin-antd-theme-ng)

## Usage

Configure in `config/theme.config.json`,

```json
{
  "theme": [
    {
      "theme": "dark",
      "fileName": "dark.css"
    },
    {
      "fileName": "mingQing.css",
      "modifyVars": {
        "@primary-color": "#13C2C2"
      }
    }
  ],
  // 是否压缩css
  "min": true,
  // css module
  "isModule": true,
  // 忽略 antd 的依赖
  "ignoreAntd": false,
  // 忽略 pro-layout
  "ignoreProLayout": false,
  // 不使用缓存
  "cache": true
}
```

Configure in `config/theme.config.js`,

```js
const theme = {
  "theme": [
    {
      "theme": "dark",
      "fileName": "dark.css"
    },
    {
      "fileName": "mingQing.css",
      "modifyVars": {
        "@primary-color": "#13C2C2"
      }
    }
  ],
  // 是否压缩css
  "min": true,
  // css module
  "isModule": true,
  // 忽略 antd 的依赖
  "ignoreAntd": false,
  // 忽略 pro-layout
  "ignoreProLayout": false,
  // 不使用缓存
  "cache": true
}

module.exports = theme;

```

you can get config in `window.umi_plugin_ant_themeVar`

## LICENSE

MIT
