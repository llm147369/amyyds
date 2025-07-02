# 🌟 阿铭的个人主页

一个基于现代新拟态设计风格的响应式个人主页，具有精美的动画效果和交互体验。

## 🎯 在线访问

📱 **GitHub Pages**: [https://llm147369.github.io/amyyds/](https://llm147369.github.io/amyyds/)

## ✨ 特色功能

### 🎨 设计特色
- **新拟态设计**: 采用现代Neumorphism设计风格
- **响应式布局**: 完美适配桌面端、平板和移动设备
- **流畅动画**: CSS3动画和过渡效果
- **渐变色彩**: 精美的渐变色按钮设计

### 🚀 交互体验
- **智能卡片**: 鼠标悬停或点击展开个人信息
- **触摸优化**: 支持移动端滑动手势
- **键盘导航**: 完整的键盘无障碍支持
- **图标集成**: Bootstrap Icons图标库

### 📊 个人信息展示
- 个人头像和简介
- 社交媒体统计数据
- 多平台社交链接
- 联系方式

## 🛠️ 技术栈

- **HTML5**: 语义化标签，SEO优化
- **CSS3**: 
  - CSS Grid 和 Flexbox 布局
  - CSS Variables (自定义属性)
  - 响应式媒体查询
  - 新拟态阴影效果
- **JavaScript**: 
  - 原生JS交互功能
  - 触摸事件处理
  - 图片预加载优化
- **Bootstrap Icons**: 矢量图标库

## 📱 响应式设计

### 桌面端 (>768px)
- 卡片尺寸: 600px 最大宽度
- 头像: 180px → 250px (展开时)
- 社交按钮: 2列网格布局

### 平板端 (≤768px)
- 优化间距和字体大小
- 调整卡片高度
- 头像: 150px → 200px (展开时)

### 移动端 (≤480px)
- 社交按钮: 单列布局
- 紧凑的内容布局
- 触摸友好的交互区域

## 🔧 优化特性

### 性能优化
- **字体预加载**: 关键字体资源预加载
- **图片懒加载**: `loading="lazy"` 属性
- **CSS优化**: 使用CSS变量减少重复代码
- **动画优化**: 硬件加速的CSS动画

### SEO优化
- **Meta标签**: 完整的SEO meta信息
- **Open Graph**: 社交分享优化
- **语义化HTML**: 提升搜索引擎理解
- **Alt属性**: 图片无障碍描述

### 无障碍改进
- **ARIA标签**: 屏幕阅读器支持
- **键盘导航**: Tab和Enter/Space支持
- **焦点指示**: 清晰的焦点样式
- **动画控制**: 尊重用户的动画偏好设置

## 📁 项目结构

```
amyyds/
├── index.html          # 主页文件
├── tx.jpg             # 个人头像
├── icon.jpg           # 个人图标
├── README.md          # 项目说明
└── .github/
    └── workflows/
        └── deploy.yml # GitHub Actions部署配置
```

## 🚀 部署步骤

### GitHub Pages 部署

1. **Fork 或 Clone 项目**
```bash
git clone https://github.com/llm147369/amyyds.git
cd amyyds
```

2. **启用 GitHub Pages**
   - 进入仓库设置页面
   - 找到 "Pages" 选项
   - 选择 "Deploy from a branch"
   - 选择 "main" 分支
   - 点击 "Save"

3. **自动部署**
   - 每次推送到 main 分支会自动部署
   - 访问: `https://your-username.github.io/amyyds/`

### 本地开发

```bash
# 使用 Python 启动本地服务器
python3 -m http.server 8080

# 或使用 Node.js
npx serve .

# 访问 http://localhost:8080
```

## 🔄 自定义修改

### 修改个人信息
编辑 `index.html` 文件中的以下内容：

1. **基本信息**:
```html
<h1>你的名字 <img src="your-icon.jpg" alt="个人图标" class="icon"></h1>
<p class="motto">你的个人座右铭</p>
```

2. **统计数据**:
```html
<div class="stat-number">你的数据</div>
<div class="stat-label">数据标签</div>
```

3. **社交链接**:
```html
<a href="你的链接" class="social-btn">
    <i class="bi bi-图标名称"></i>
    平台名称
</a>
```

### 替换图片
- 替换 `tx.jpg` 为你的头像 (建议尺寸: 400x400px)
- 替换 `icon.jpg` 为你的个人图标 (建议尺寸: 100x100px)

## 🎨 自定义样式

通过修改CSS变量快速定制主题：

```css
:root {
    --primary-bg: #E0E0E0;        /* 主背景色 */
    --text-primary: #3C1B38;      /* 主文字颜色 */
    --text-secondary: #351C0A;    /* 次要文字颜色 */
    /* 更多变量... */
}
```

## 📝 更新日志

### v2.0.0 (2024-07-02)
- ✨ 完全重构，采用现代化设计
- 🎨 新增新拟态设计风格
- 📱 全面响应式支持
- ♿ 无障碍改进
- 🚀 性能优化
- 🔧 SEO优化

### v1.0.0 (2023-10-10)
- 🎉 初始版本发布
- 💫 基础卡片动画效果

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

## 📄 许可证

MIT License - 详见 [LICENSE](LICENSE) 文件

## 🙏 致谢

- [Bootstrap Icons](https://icons.getbootstrap.com/) - 图标库
- [HarmonyOS Sans](https://developer.harmonyos.com/) - 字体支持

---

⭐ 如果这个项目对你有帮助，请给它一个星标！