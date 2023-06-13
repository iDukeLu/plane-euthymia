# plane-euthymia
基于 Docusaurus 搭建的静态文档站。

## 部署 GitHub Pages

### 部署配置
修改 *docusaurus.config.js* 配置
```
module.exports = {
  // ...
  url: 'https://idukelu.github.io',  // Your website URL
  baseUrl: '/plane-euthymia',        // For GitHub pages deployment, it is often '/<projectName>/'
  organizationName: 'iDukeLu',       // Usually your GitHub org/user name.
  projectName: 'plane-euthymia',     // Usually your repo name.
  trailingSlash: false,
  // ...
};
```
更多可参考：https://docusaurus.io/zh-CN/docs/deployment#docusaurusconfigjs-settings

### 部署命令
使用 SSH 进行部署，避免每次都输密码
```
GIT_USER=idukelu USE_SSH=true yarn deploy
```
其他环境参数可参考：https://docusaurus.io/zh-CN/docs/deployment#environment-settings