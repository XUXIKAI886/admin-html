# 贡献指南

感谢您对 Gleek Bootstrap Admin Dashboard 项目的关注！我们欢迎所有形式的贡献，包括但不限于：

- 🐛 报告 Bug
- 💡 提出新功能建议
- 📝 改进文档
- 🔧 提交代码修复
- 🎨 UI/UX 改进建议
- 🌍 国际化翻译

## 📋 贡献方式

### 报告问题 🐛

如果您发现了 Bug 或有改进建议，请：

1. 检查 [Issues](https://github.com/XUXIKAI886/admin-html/issues) 确保问题未被报告
2. 使用清晰的标题描述问题
3. 提供详细的问题描述，包括：
   - 操作系统和浏览器版本
   - 重现步骤
   - 期望行为
   - 实际行为
   - 截图（如适用）

### 提交代码 💻

1. **Fork 仓库**
   ```bash
   # 点击 GitHub 页面右上角的 Fork 按钮
   ```

2. **克隆您的 Fork**
   ```bash
   git clone https://github.com/YOUR_USERNAME/admin-html.git
   cd admin-html
   ```

3. **创建特性分支**
   ```bash
   git checkout -b feature/amazing-feature
   # 或
   git checkout -b bugfix/fix-issue-123
   ```

4. **安装依赖**
   ```bash
   npm install
   ```

5. **进行更改**
   - 遵循项目的代码规范
   - 添加必要的测试
   - 更新相关文档

6. **提交更改**
   ```bash
   git add .
   git commit -m "feat: 添加令人惊叹的新功能"
   ```

7. **推送到您的 Fork**
   ```bash
   git push origin feature/amazing-feature
   ```

8. **创建 Pull Request**
   - 访问您的 Fork 页面
   - 点击 "New Pull Request"
   - 填写详细的 PR 描述

## 📝 代码规范

### HTML 规范
```html
<!-- 使用语义化标签 -->
<header class="main-header">
  <nav class="navbar navbar-expand-lg">
    <div class="container-fluid">
      <!-- 内容 -->
    </div>
  </nav>
</header>

<!-- 使用 2 个空格缩进 -->
<div class="card">
  <div class="card-header">
    <h4 class="card-title">标题</h4>
  </div>
  <div class="card-body">
    <!-- 内容 -->
  </div>
</div>
```

### CSS/SCSS 规范
```scss
// 使用 BEM 命名规范
.card {
  border-radius: 0.5rem;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  
  &__header {
    padding: 1rem;
    border-bottom: 1px solid #e9ecef;
  }
  
  &__body {
    padding: 1rem;
  }
  
  &--highlighted {
    border: 2px solid #007bff;
  }
}

// 使用变量
$primary-color: #007bff;
$border-radius: 0.5rem;
$spacing-unit: 1rem;

// 使用 mixins
@mixin button-style($bg-color, $text-color) {
  background-color: $bg-color;
  color: $text-color;
  border: none;
  border-radius: $border-radius;
  padding: 0.5rem $spacing-unit;
}
```

### JavaScript 规范
```javascript
// 使用 ES6+ 语法
const initializeChart = (element, data) => {
  const config = {
    type: 'bar',
    data: data,
    options: {
      responsive: true,
      maintainAspectRatio: false
    }
  };
  
  return new Chart(element, config);
};

// 使用 JSDoc 注释
/**
 * 初始化仪表板组件
 * @param {Object} options - 配置选项
 * @param {string} options.theme - 主题名称
 * @param {boolean} options.responsive - 是否响应式
 */
const initDashboard = (options = {}) => {
  const defaults = {
    theme: 'light',
    responsive: true
  };
  
  const settings = { ...defaults, ...options };
  
  // 实现逻辑
};

// 使用现代 JavaScript 特性
class ThemeManager {
  constructor(options) {
    this.options = options;
    this.currentTheme = 'light';
  }
  
  setTheme(theme) {
    this.currentTheme = theme;
    document.body.className = `theme-${theme}`;
  }
  
  toggleTheme() {
    const newTheme = this.currentTheme === 'light' ? 'dark' : 'light';
    this.setTheme(newTheme);
  }
}
```

## 🎯 提交信息规范

使用 [Conventional Commits](https://www.conventionalcommits.org/) 规范：

```
<类型>[可选的作用域]: <描述>

[可选的正文]

[可选的脚注]
```

### 类型说明
- `feat`: 新功能
- `fix`: Bug 修复
- `docs`: 文档更新
- `style`: 代码格式调整（不影响功能）
- `refactor`: 代码重构
- `perf`: 性能优化
- `test`: 测试相关
- `chore`: 构建过程或辅助工具的变动

### 示例
```bash
feat(dashboard): 添加新的加密货币仪表板模板

- 添加比特币价格图表
- 集成交易量统计
- 支持多种加密货币切换

Closes #123
```

## 🧪 测试指南

### 浏览器测试
确保您的更改在以下浏览器中正常工作：
- Chrome (最新版本)
- Firefox (最新版本)
- Safari (最新版本)
- Edge (最新版本)

### 响应式测试
测试以下设备尺寸：
- 手机: 320px - 767px
- 平板: 768px - 1023px
- 桌面: 1024px+

### 功能测试
- 确保所有链接正常工作
- 验证表单提交功能
- 测试 JavaScript 交互
- 检查图表和组件渲染

## 📚 文档贡献

### 改进现有文档
- 修正拼写和语法错误
- 添加缺失的信息
- 改进代码示例
- 更新过时的内容

### 添加新文档
- 新功能使用指南
- 最佳实践文档
- 故障排除指南
- 国际化翻译

## 🌍 国际化

我们欢迎多语言支持的贡献：

1. 复制 `docs/en/` 目录
2. 重命名为目标语言代码（如 `docs/zh/`）
3. 翻译所有文档内容
4. 更新导航链接

## 🎨 设计贡献

### UI/UX 改进
- 提供设计稿或原型
- 改进用户体验流程
- 优化视觉设计
- 提升可访问性

### 图标和图片
- 提供高质量的图标
- 优化现有图片
- 添加新的插图

## 📞 联系方式

如果您有任何问题或需要帮助：

- **GitHub Issues**: [提交问题](https://github.com/XUXIKAI886/admin-html/issues)
- **邮箱**: quixlab.com@gmail.com
- **Skype**: sporsho9

## 🏆 贡献者

感谢所有为项目做出贡献的开发者！

<!-- 这里将自动生成贡献者列表 -->

## 📄 许可证

通过贡献代码，您同意您的贡献将在与项目相同的许可证下发布。

---

再次感谢您的贡献！每一个贡献都让 Gleek 变得更好。 🚀
