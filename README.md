# atcumt-2015
> 文档分析：Claude Sonnet 4.5
> 生成日期：2025-11-02

翔工作室主页2015：https://www.atcumt.com/atcumt-2015
```main```分支为源码备份，```release/2026```分支为后期修改发布版本。

|![](https://raw.githubusercontent.com/cumtflyingstudio/atcumt-pic/main/web/atcumt-2015-m.png)|![](https://raw.githubusercontent.com/cumtflyingstudio/atcumt-pic/main/web/atcumt-2015-pc.png)|
|:---:|:---:|

## 项目简介

这是一个基于静态文件的前端网站仓库，包含主页 `index.html` 及相关的资源目录（`css/`、`js/`、`img/`、`font/`、`video/`）,适合部署到 GitHub Pages 或任意静态站点托管服务。

## 项目架构

```
atcumt-2015/
├── index.html            # 站点首页
├── css/                  # 样式（reset + index）
│   ├── reset.css
│   ├── index.css
│   └── index - 副本.css  # 副本/备份样式文件
├── js/                   # 前端脚本
│   ├── index.js
│   ├── function.js
│   └── screenEnterLeave.js
├── font/                 # 字体文件
│   └── ebrimabd.ttf
├── img/                  # 图片资源（logo、封面、图标等）
├── video/                # 视频资源 (1.mp4)
└── README.md             # 本文件
```

### 核心功能/目录

#### `index.html`
 - 作为单页展示入口，引用 `css` 和 `js` 资源，负责页面布局和交互触发。

#### `css/`
 - `reset.css` 用于重置浏览器默认样式，`index.css` 为主样式表。目录中存在 `index - 副本.css`，看起来是样式备份，应在开发流程中清理或合并。

#### `js/`
 - `index.js`：主脚本，负责页面交互逻辑
 - `function.js`：通用辅助函数
 - `screenEnterLeave.js`：可能用于视口/动画进入离开效果

#### `img/` 和 `font/`
 - 图片与字体用于视觉展示和品牌标识，注意检查是否有未使用或重复资源以减小站点体积。

#### `video/`
 - 存放媒体资源（例如 `1.mp4`），在网页中使用视频时请注意跨浏览器兼容性.
### 工程化配置

当前仓库为纯静态站点，未发现构建工具（如 npm、webpack、gulp 等）或 CI 配置（如 GitHub Actions）。如需自动化部署和压缩/打包，可考虑引入简单的 npm 脚本或 GitHub Actions。

## 许可证

本项目采用 Apache License 2.0 许可，详见仓库根目录的 `LICENSE` 文件。