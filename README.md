# Gleek - Bootstrap 4 管理后台 HTML 模板

<div align="center">
  <img src="gleek/assets/images/logo.png" alt="Gleek Logo" width="200">
  
  [![Bootstrap](https://img.shields.io/badge/Bootstrap-4.1.3-7952b3?style=flat-square&logo=bootstrap)](https://getbootstrap.com/)
  [![License](https://img.shields.io/badge/License-ThemeForest-green?style=flat-square)](https://themeforest.net/licenses/terms/regular)
  [![Version](https://img.shields.io/badge/Version-1.0.0-blue?style=flat-square)](https://github.com/XUXIKAI886/admin-html)
  [![Node.js](https://img.shields.io/badge/Node.js-Required-339933?style=flat-square&logo=node.js)](https://nodejs.org/)
</div>

## 📖 项目简介

Gleek 是一个功能强大、响应式的 Bootstrap 4 管理后台 HTML 模板，专为现代 Web 应用程序设计。它提供了 22 种不同行业的仪表板风格，100+ 个插件集成，以及完整的 UI 组件库，是构建专业管理系统的理想选择。

## ✨ 主要特性

### 🎨 多样化仪表板
- **22种行业模板** - 餐厅、医院、学校、电商、加密货币等
- **响应式设计** - 完美适配桌面、平板、手机
- **现代化界面** - 扁平化设计风格，用户体验优秀

### 🛠️ 技术栈
- **Bootstrap 4.1.3** - 最新的前端框架
- **SASS/SCSS** - 模块化样式预处理器
- **Gulp** - 自动化构建工具
- **jQuery 3.3.1** - JavaScript 库
- **100+ 插件** - 图表、表单、UI组件等

### 📊 丰富组件
- **14种图表库** - Chart.js、Highcharts、Morris.js 等
- **多种表格** - DataTables、Bootstrap Tables、JSGrid 等
- **表单组件** - 日期选择器、文件上传、富文本编辑器等
- **UI元素** - 按钮、卡片、模态框、导航等

## 🚀 快速开始

### 环境要求
- Node.js (推荐 v12.0.0 或更高版本)
- npm 或 yarn 包管理器
- 现代浏览器 (Chrome, Firefox, Safari, Edge)

### 安装步骤

1. **克隆项目**
```bash
git clone https://github.com/XUXIKAI886/admin-html.git
cd admin-html
```

2. **安装依赖**
```bash
npm install
```

3. **启动开发服务器**
```bash
npm start
```

4. **访问项目**
打开浏览器访问 `http://localhost:8080`

### 构建生产版本

```bash
# 编译 SASS
npm run sass

# 使用 Gulp 构建
gulp plugin
gulp common_js
```

## 📁 项目结构

```
htmlyuanma/
├── documentation/          # 项目文档
│   ├── index.html         # 文档主页
│   ├── css/               # 文档样式
│   └── images/            # 文档图片
├── gleek/                 # 主要模板文件
│   ├── assets/            # 静态资源
│   │   ├── images/        # 图片资源
│   │   └── plugins/       # 第三方插件
│   └── main/              # 核心文件
│       ├── css/           # 编译后的CSS
│       ├── js/            # JavaScript文件
│       ├── scss/          # SASS源文件
│       ├── icons/         # 图标字体
│       └── template/      # HTML模板
├── package.json           # 项目配置
├── gulpfile.js           # Gulp配置
└── README.md             # 项目说明
```

## 🎯 仪表板风格

### 行业模板
| 模板名称 | 文件名 | 适用场景 |
|---------|--------|----------|
| 餐厅管理 | `index-restaurent.html` | 餐饮业管理系统 |
| 医院管理 | `index-hospital.html` | 医疗机构管理 |
| 学校管理 | `index-school.html` | 教育机构管理 |
| 电商管理 | `index-product.html` | 电子商务平台 |
| 加密货币 | `index-crypto.html` | 数字货币交易 |
| 房地产 | `index-real-estate.html` | 房产管理系统 |
| 健身中心 | `index-fitness.html` | 健身房管理 |
| 音乐平台 | `index-music.html` | 音乐流媒体 |
| 博客管理 | `index-blog.html` | 内容管理系统 |
| 活动管理 | `index-events.html` | 活动策划管理 |

### 布局选项
- **垂直布局** / **水平布局**
- **固定头部** / **静态头部**
- **左侧边栏** / **右侧边栏**
- **浅色主题** / **深色主题**
- **盒式布局** / **全宽布局**

## 🔧 自定义配置

### 主题配置
在 `gleek/main/js/gleek.js` 中配置主题选项：

```javascript
new quixSettings({
    version: "light",              // light | dark
    layout: "vertical",            // vertical | horizontal
    sidebarStyle: "full",          // full | mini | compact | overlay
    sidebarPosition: "fixed",      // static | fixed
    headerPosition: "fixed",       // static | fixed
    containerLayout: "wide",       // wide | boxed | wide-boxed
    direction: "ltr",              // ltr | rtl
    navheaderBg: "color_1",       // color_1 到 color_10
    headerBg: "color_1",          // color_1 到 color_10
    sidebarBg: "color_1"          // color_1 到 color_10
});
```

### SASS 编译
```bash
# 监听文件变化并自动编译
npm run sass

# 或使用 node-sass 直接编译
node-sass --watch gleek/main/scss/main.scss gleek/main/css/style.css
```

## 📚 组件文档

### 图表组件
- **Chart.js** - 现代化图表库
- **Highcharts** - 专业图表解决方案
- **Morris.js** - 简洁的线图和柱状图
- **C3.js** - 基于 D3.js 的图表库
- **ECharts** - 百度开源图表库

### 表单组件
- **日期选择器** - Bootstrap Datepicker, Material Datepicker
- **文件上传** - Dropzone, Dropify
- **富文本编辑器** - Summernote, CKEditor, TinyMCE
- **表单验证** - Bootstrap Validator, jQuery Validation

### UI 组件
- **数据表格** - DataTables, Bootstrap Tables
- **模态框** - Bootstrap Modal, SweetAlert
- **通知组件** - Toastr, Bootstrap Notify
- **进度条** - 圆形进度条, 线性进度条

## 🌐 浏览器支持

| 浏览器 | 版本支持 |
|--------|----------|
| Chrome | 60+ |
| Firefox | 55+ |
| Safari | 11+ |
| Edge | 16+ |
| IE | 11+ |

## 📱 响应式断点

```scss
// 超小屏幕 (手机)
@media (max-width: 575.98px) { ... }

// 小屏幕 (手机横屏)
@media (min-width: 576px) and (max-width: 767.98px) { ... }

// 中等屏幕 (平板)
@media (min-width: 768px) and (max-width: 991.98px) { ... }

// 大屏幕 (桌面)
@media (min-width: 992px) and (max-width: 1199.98px) { ... }

// 超大屏幕 (大桌面)
@media (min-width: 1200px) { ... }
```

## 🔌 插件列表

### 图表插件 (14个)
- Chart.js, Highcharts, Morris.js, C3.js, ECharts
- Flot, Chartist, Sparkline, Rickshaw, Peity
- JustGage, Knob, Circle Progress, Easy Pie Chart

### 表单插件 (23个)
- Smart Wizard, Form Step, Summernote, CKEditor
- Quill Editor, TinyMCE, Date Picker, Clock Picker
- Color Picker, Material Design, Dropzone, Touch Spinner
- Select2, Input Mask, Switch, Tag Input, Type Head
- xEditable, Dropify, Cropper, Bootstrap Validate, jQuery Validate

### 表格插件 (5个)
- DataTables, Bootstrap Tables, JSGrid, Foo Tables, Boot Grid

### UI插件 (50+个)
- Block UI, Bootstrap Notify, Clipboard, Sweet Alert
- Toastr, Magnific Popup, Owl Carousel, 等等...

## 🎨 主题定制

### 颜色方案
模板提供 10 种预设颜色方案：
- `color_1` - 默认蓝色
- `color_2` - 绿色
- `color_3` - 橙色
- `color_4` - 紫色
- `color_5` - 红色
- `color_6` - 青色
- `color_7` - 粉色
- `color_8` - 黄色
- `color_9` - 深蓝色
- `color_10` - 深绿色

### 自定义样式
```scss
// 在 custom.scss 中添加自定义样式
.custom-component {
    background-color: #your-color;
    border-radius: 8px;
    padding: 1rem;
}
```

## 📋 使用示例

### 创建新页面
1. 复制 `template/layout-starter-kit.html`
2. 修改页面标题和内容
3. 添加所需的CSS和JS文件
4. 自定义页面布局和组件

### 集成图表
```html
<!-- 引入Chart.js -->
<script src="../assets/plugins/chart.js/Chart.bundle.min.js"></script>

<!-- HTML容器 -->
<canvas id="myChart"></canvas>

<!-- JavaScript配置 -->
<script>
var ctx = document.getElementById('myChart').getContext('2d');
var myChart = new Chart(ctx, {
    type: 'bar',
    data: {
        labels: ['一月', '二月', '三月', '四月', '五月', '六月'],
        datasets: [{
            label: '销售数据',
            data: [12, 19, 3, 5, 2, 3],
            backgroundColor: 'rgba(54, 162, 235, 0.2)',
            borderColor: 'rgba(54, 162, 235, 1)',
            borderWidth: 1
        }]
    }
});
</script>
```

## 🚀 部署指南

### 静态部署
1. 构建项目：`npm run build`
2. 将 `dist/` 目录上传到服务器
3. 配置 Web 服务器指向 `index.html`

### 推荐部署平台
- **Netlify** - 免费静态网站托管
- **Vercel** - 现代化部署平台
- **GitHub Pages** - GitHub 免费托管
- **Firebase Hosting** - Google 云托管

## 🤝 贡献指南

我们欢迎社区贡献！请遵循以下步骤：

1. Fork 本仓库
2. 创建特性分支：`git checkout -b feature/AmazingFeature`
3. 提交更改：`git commit -m 'Add some AmazingFeature'`
4. 推送分支：`git push origin feature/AmazingFeature`
5. 提交 Pull Request

### 代码规范
- 使用 2 个空格缩进
- 遵循 BEM CSS 命名规范
- JavaScript 使用 ES6+ 语法
- 提交信息使用中文描述

## 📄 许可证

本项目基于 [ThemeForest Regular License](https://themeforest.net/licenses/terms/regular) 许可证。

## 👥 开发团队

- **开发者**: [Quixlab](https://themeforest.net/user/quixlab)
- **设计师**: [DigitalHeaps](https://themeforest.net/user/digitalheaps)
- **技术支持**: quixlab.com@gmail.com
- **Skype**: sporsho9

## 🔗 相关链接

- [在线演示](https://your-demo-link.com)
- [官方文档](./documentation/index.html)
- [技术支持](mailto:quixlab.com@gmail.com)
- [更新日志](./CHANGELOG.md)

## ❓ 常见问题

### Q: 如何更改默认主题颜色？
A: 在 `gleek/main/js/gleek.js` 文件中修改 `navheaderBg`、`headerBg`、`sidebarBg` 参数。

### Q: 如何添加新的页面？
A: 复制 `template/layout-starter-kit.html` 作为模板，然后根据需要修改内容。

### Q: 支持 RTL（从右到左）布局吗？
A: 是的，在配置中设置 `direction: "rtl"` 即可启用 RTL 支持。

### Q: 如何自定义 SASS 变量？
A: 在 `gleek/main/scss/abstracts/_variables.scss` 中修改相关变量。

---

<div align="center">
  <p>如果这个项目对您有帮助，请给我们一个 ⭐ Star！</p>
  <p>© 2024 Gleek Admin Template. All rights reserved.</p>
</div>
