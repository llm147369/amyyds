# 🌟 阿铭的现代化个人网站

一个采用现代新拟态设计风格的专业个人网站，具有悬浮式导航、多页面布局和精美的交互动画。

## 🎯 在线访问

� **GitHub Pages**: [https://llm147369.github.io/amyyds/](https://llm147369.github.io/amyyds/)

![Website Preview](https://img.shields.io/badge/Status-Live-brightgreen) ![Design](https://img.shields.io/badge/Design-Neumorphism-blueviolet) ![Responsive](https://img.shields.io/badge/Responsive-Yes-success)

## ✨ 核心特性

### 🧭 现代新拟态导航栏
- **悬浮式设计**: 固定在页面顶部的浮动导航
- **模糊背景**: backdrop-filter 模糊效果
- **智能响应**: 自适应汉堡菜单
- **活动指示**: 动态高亮当前页面
- **平滑切换**: 丝滑的过渡动画

### � 五大核心页面
1. **🏠 首页** - 个人介绍和英雄区域
2. **👤 关于** - 技能展示和专业背景
3. **⚙️ 服务** - 提供的专业服务
4. **💼 作品** - 项目作品集展示
5. **📧 联系** - 联系信息和表单

### 🎨 新拟态设计系统
- **深度阴影**: 多层次的光影效果
- **内嵌样式**: inset 阴影创造凹陷感
- **悬停反馈**: 立体的交互动画
- **渐变配色**: 精心调制的色彩方案

## 🛠️ 技术架构

### 前端技术栈
- **HTML5**: 语义化标签结构
- **CSS3**: 
  - CSS Variables (自定义属性系统)
  - CSS Grid & Flexbox 现代布局
  - Backdrop-filter 模糊效果
  - Transform3D 硬件加速
- **Vanilla JavaScript**: 
  - Intersection Observer API
  - 平滑滚动导航
  - 响应式交互

### 设计系统
```css
:root {
  /* 颜色系统 */
  --bg-primary: #f0f2f5;
  --shadow-light: #ffffff;
  --shadow-dark: #d1d9e6;
  
  /* 渐变色板 */
  --gradient-primary: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  --gradient-secondary: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
  
  /* 间距系统 */
  --space-xs: 0.5rem;
  --space-xl: 3rem;
  
  /* 动画时间 */
  --transition-fast: 0.2s ease;
  --transition-slow: 0.5s ease;
}
```

## 🎯 设计亮点

### 🔄 交互动画
- **滚动触发**: 元素进入视野时的淡入动画
- **悬停效果**: 立体的阴影变化
- **导航切换**: 平滑的页面滚动
- **表单反馈**: 实时的视觉响应

### � 响应式体验
| 设备类型 | 屏幕宽度 | 导航样式 | 布局调整 |
|---------|----------|----------|----------|
| 桌面端 | >768px | 水平导航 | 多列网格 |
| 平板端 | ≤768px | 收起菜单 | 调整间距 |
| 移动端 | ≤480px | 汉堡菜单 | 单列布局 |

### 🎨 视觉层次
```
页面结构层次:
├── 悬浮导航栏 (z-index: 1000)
├── 英雄区域 (全屏高度)
├── 内容区域 (卡片布局)
└── 交互元素 (悬停态)
```

## 🚀 功能展示

### 🧭 智能导航系统
```javascript
// 自动更新活动状态
function updateActiveNav() {
  const scrollPos = window.scrollY + 150;
  sections.forEach(section => {
    // 检测当前可视区域
    if (scrollPos >= sectionTop && scrollPos < sectionTop + sectionHeight) {
      // 更新导航状态
      updateNavigation(sectionId);
    }
  });
}
```

### 🎬 滚动动画系统
```javascript
// Intersection Observer 实现
const observer = new IntersectionObserver((entries) => {
  entries.forEach(entry => {
    if (entry.isIntersecting) {
      entry.target.classList.add('visible');
    }
  });
}, { threshold: 0.1 });
```

## � 性能优化

### ⚡ 加载优化
- **字体预加载**: 关键字体提前下载
- **图片懒加载**: 按需加载策略
- **CSS优化**: 变量复用减少重复
- **JS压缩**: 精简的脚本代码

### 🔧 代码质量
- **模块化CSS**: 组件化样式结构
- **语义化HTML**: 提升可访问性
- **现代JS**: ES6+ 语法特性
- **性能监控**: Lighthouse 优化

## 🎨 定制指南

### 🔧 快速个性化

1. **修改个人信息**:
```html
<h1 class="hero-title">你好，我是[姓名]</h1>
<p class="hero-subtitle">[职业描述]</p>
```

2. **更换配色方案**:
```css
:root {
  --gradient-primary: linear-gradient(135deg, [颜色1], [颜色2]);
  --text-accent: [主题色];
}
```

3. **添加项目作品**:
```html
<div class="card fade-in">
  <div class="card-icon" style="background: var(--gradient-primary);">
    <i class="bi bi-[图标名]"></i>
  </div>
  <h3 class="card-title">[项目名称]</h3>
  <p class="card-description">[项目描述]</p>
</div>
```

### 🖼️ 资源替换
- **头像图片**: 替换 `tx.jpg` (推荐 400x400px)
- **图标文件**: 替换 `icon.jpg` (推荐 100x100px)
- **社交链接**: 更新 href 属性为实际链接

## 🔗 社交链接配置

```html
<!-- 示例配置 -->
<a href="https://github.com/your-username" class="social-link">
  <i class="bi bi-github"></i>
</a>
<a href="mailto:your-email@domain.com" class="social-link">
  <i class="bi bi-envelope"></i>
</a>
```

## 📱 移动端优化

### 触摸交互
- **触摸目标**: 最小44px点击区域
- **手势支持**: 滑动导航
- **性能优化**: 硬件加速动画

### 视觉适配
- **动态字体**: rem单位响应式缩放
- **灵活布局**: 网格自适应重排
- **触摸反馈**: 即时的视觉响应

## 🔄 版本更新

### v3.0.0 (2024-07-02) - 🎨 现代重构
- ✨ **全新导航**: 悬浮式新拟态导航栏
- 🏗️ **架构升级**: 多页面单页应用结构
- 🎨 **设计系统**: CSS变量驱动的设计
- 📱 **响应式**: 完整的移动端适配
- � **性能**: Intersection Observer优化

### v2.0.0 (2024-07-02) - 🔧 功能完善
- 🎨 新拟态设计风格
- 📱 响应式布局优化
- ♿ 无障碍功能增强

### v1.0.0 (2023-10-10) - 🎉 初始版本
- 💫 基础卡片动画效果

## 🚀 部署指南

### GitHub Pages 部署
1. Fork 此仓库
2. 启用 GitHub Pages (Settings → Pages)
3. 选择 main 分支作为源
4. 访问 `https://your-username.github.io/amyyds/`

### 本地开发
```bash
# 启动本地服务器
python3 -m http.server 8080
# 或
npx serve .

# 访问 http://localhost:8080
```

## 🌐 浏览器支持

| 浏览器 | 版本 | 支持状态 |
|--------|------|----------|
| Chrome | 88+ | ✅ 完全支持 |
| Firefox | 84+ | ✅ 完全支持 |
| Safari | 14+ | ✅ 完全支持 |
| Edge | 88+ | ✅ 完全支持 |

## 🤝 贡献指南

欢迎提交 Issues 和 Pull Requests！

### 开发规范
- 遵循现有的代码风格
- 保持响应式设计原则
- 添加适当的注释说明
- 测试多设备兼容性

## 📄 许可证

MIT License - 详见 [LICENSE](LICENSE) 文件

## 🙏 致谢

- [Inter Font](https://rsms.me/inter/) - 现代化字体
- [Bootstrap Icons](https://icons.getbootstrap.com/) - 图标库
- [CSS Tricks](https://css-tricks.com/) - 技术参考
- [Neumorphism Design](https://neumorphism.io/) - 设计灵感

## 📈 统计信息

![GitHub stars](https://img.shields.io/github/stars/llm147369/amyyds?style=social)
![GitHub forks](https://img.shields.io/github/forks/llm147369/amyyds?style=social)
![GitHub issues](https://img.shields.io/github/issues/llm147369/amyyds)
![GitHub last commit](https://img.shields.io/github/last-commit/llm147369/amyyds)

---

⭐ **如果这个项目对您有帮助，请给它一个星标！**

🔥 **现代化设计 × 专业级代码 × 完美响应式 = 您的理想个人网站**