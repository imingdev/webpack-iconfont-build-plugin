# webpack-iconfont-build-plugin

在 webpack 项目中引入 Iconfont

安装

```sh
npm i webpack-iconfont-build-plugin -D
```

在 Iconfont 上找到你项目的 CSS 地址

![image](https://user-images.githubusercontent.com/20639676/81887919-c9d3e780-95d2-11ea-8455-27a3cc6964a7.png)

然后将插件加入到 `webpack.config.js` 中

```js
const WebpackIconfontPlugin = require("webpack-iconfont-build-plugin");
module.exports = {
  plugins: [
    WebpackIconfontPlugin({
      // 将上面的CSS加入到此处
      cssURL: "http://at.alicdn.com/t/font_8d5l8fzk5b87iudi.css"
    })
  ]
};
```

使用

```html
<i class="icon-zhifubao" />
```

