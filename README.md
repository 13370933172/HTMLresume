# HTMLresume

基于 [MDUI](https://www.mdui.org/)（Material Design UI）框架构建的个人简历/作品集静态网站。

## 功能特性

- **个人信息展示**：姓名、电话、邮箱等基本信息
- **语言能力**：使用进度条直观展示编程语言掌握程度
- **社交媒体链接**：QQ、微信、邮箱等联系方式
- **工作经历**：按时间线展示过往工作经历
- **专业技能**：展示专业技能列表
- **项目经历**：展示参与或主导的项目详情
- **响应式布局**：适配桌面端和移动端不同屏幕尺寸
- **Material Design 风格**：采用 MDUI 框架，提供现代化 UI 体验
- **动态背景**：支持自定义背景图片，带有半透明遮罩层

## 项目结构

```
HTMLresume/
├── index.html              # 主页面
├── assets/
│   ├── css/
│   │   ├── main.css        # 主样式文件（背景、布局等）
│   │   └── index.css       # 内容区域样式文件
│   ├── img/                # 背景图片资源
│   └── js/
│       └── main.js         # 主脚本文件
├── css/
│   └── font_1625701_q2422cy34wn.css  # 图标字体样式
├── imgs/
│   └── profilePicture.jpg  # 头像/Logo 图片
└── mdui/                   # MDUI 框架文件
    ├── css/                # MDUI 样式文件
    ├── fonts/              # Roboto 字体文件
    ├── icons/              # Material Icons 图标字体
    └── js/                 # MDUI JavaScript 文件
```

## 快速开始

1. 克隆或下载本项目到本地
2. 用浏览器直接打开 `index.html` 即可预览
3. 如需部署到服务器，将整个目录上传至 Web 服务器的静态文件目录即可

## 自定义配置

### 修改个人信息

编辑 `index.html` 文件，替换其中的占位内容（如 `XXX`、`123@qq.com` 等）为你自己的信息：

- **姓名/头衔**：修改 `.rin-left-title` 和 `.rin-left-title2` 中的文本
- **个人介绍**：修改 `#introduce` 区域的内容
- **联系方式**：修改 `#fighting` 区域的姓名、电话、邮箱
- **语言能力**：修改进度条宽度百分比和对应语言名称
- **社交媒体**：修改 `#contact` 区域的链接地址
- **工作经历**：修改对应区域的公司名、时间和描述
- **专业技能**：修改 `#article` 区域的技能列表
- **项目经历**：修改 `#works` 区域的项目信息
- **页脚**：修改版权信息

### 修改头像

将你的头像图片替换 `imgs/profilePicture.jpg`，建议使用正方形图片。

### 修改背景

在 `assets/css/main.css` 中修改 `#rin-bg` 的 `background-image` 路径：

```css
background-image: url('../../assets/img/background12.jpg');
```

背景图片存放在 `assets/img/` 目录下，共 16 张备选图片，替换路径即可切换。

### 修改主题色

在 `index.html` 的 `<body>` 标签上修改 MDUI 主题色类名，可选值参考 [MDUI 颜色文档](https://www.mdui.org/docs/color)。

## 技术栈

- **HTML5**：页面结构
- **CSS3**：样式与动画
- **JavaScript**：交互逻辑
- **[MDUI](https://www.mdui.org/)**：Material Design 前端框架
- **图标字体**：iconfont 自定义图标

## 浏览器兼容性

支持所有现代浏览器（Chrome、Firefox、Safari、Edge 等）。

## 许可

本项目仅供个人学习和使用。