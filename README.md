# StardewWeb

一个基于Web的《星露谷物语》游戏助手和管理工具，提供农场管理、物品追踪、任务监控等功能。

## 🌟 特性

### 📱 响应式设计
- 🖥️ 支持桌面、平板和手机设备
- 📐 自适应布局，在所有屏幕尺寸下都有良好体验
- 🎨 基于Bootstrap的现代化UI设计

### 🌍 多语言支持
- 🇺🇸 英语（默认）
- 🇨🇳 简体中文
- 🔄 自动检测浏览器语言设置
- ⚡ 客户端动态翻译

### 🎮 游戏功能

#### 🏠 农场管理
- 农作物种植和收获追踪
- 动物照料提醒
- 机器状态监控
- 建筑物管理

#### 📋 任务系统
- 每日任务列表
- 任务进度追踪
- 社区中心包裹完成度
- 成就系统

#### 👥 社交系统
- NPC好感度追踪
- 生日提醒
- 礼物推荐
- 事件触发条件

#### 📦 物品管理
- 物品搜索和分类
- 背包和箱子管理
- 物品价值计算
- 生产链追踪

#### 📊 数据统计
- 收入统计
- 生产效率分析
- 游戏进度概览
- 详细报表

## 🚀 快速开始

### 环境要求
- .NET Framework 4.7.2 或更高版本
- Web浏览器（推荐Chrome、Firefox、Edge）
- 《星露谷物语》游戏（用于数据同步）

### 安装步骤

1. **克隆仓库**
   ```bash
   git clone https://github.com/Yeaowo/StardewWeb.git
   cd StardewWeb
   ```

2. **构建项目**
   ```bash
   # 使用Visual Studio打开项目文件
   # 或使用命令行构建
   dotnet build
   ```

3. **启动应用**
   ```bash
   # 启动Web服务器
   dotnet run
   ```

4. **访问应用**
   打开浏览器访问 `http://localhost:5000`

## 📖 使用指南

### 基本设置

1. **游戏数据同步**
   - 确保《星露谷物语》游戏正在运行
   - 在配置页面设置游戏数据路径
   - 启用自动数据同步

2. **语言设置**
   - 应用会自动检测浏览器语言
   - 也可在设置中手动切换语言
   - 支持英语和简体中文

3. **响应式布局**
   - 在移动设备上使用汉堡菜单导航
   - 支持触摸操作和手势
   - 自动调整字体大小和间距

### 主要功能

#### 🏡 今日概览
- 查看当前游戏状态
- 今日待办任务
- 天气和季节信息
- 快速操作按钮

#### 📈 生产管理
- 农作物成熟时间
- 动物产品收集
- 机器处理状态
- 利润优化建议

#### 🎯 任务追踪
- 主线任务进度
- 社区中心包裹
- 成就完成情况
- 收集品追踪

#### 👫 社交网络
- NPC关系管理
- 生日日历
- 礼物偏好查询
- 心情事件触发

## 🛠️ 技术栈

### 后端
- **框架**: .NET Framework / .NET Core
- **语言**: C#
- **数据访问**: Entity Framework
- **API**: RESTful Web API

### 前端
- **框架**: Bootstrap 5
- **样式**: CSS3 + 响应式设计
- **脚本**: JavaScript (ES6+)
- **字体**: Stardew Valley 主题字体

### 数据
- **格式**: JSON配置文件
- **国际化**: i18n JSON文件
- **缓存**: 内存缓存 + 本地存储

## 🌏 国际化

### 支持的语言
- **英语** (`en`): 完整支持
- **简体中文** (`zh-cn`): 完整支持

### 添加新语言

1. **创建语言文件**
   ```bash
   cp i18n/default.json i18n/[language-code].json
   ```

2. **翻译文本**
   ```json
   {
     "navbar.home": "Your Translation",
     "navbar.tasks": "Your Translation"
   }
   ```

3. **更新语言检测**
   ```javascript
   // 在 header.html 中添加新语言检测
   if (userLang.startsWith('your-language-code')) {
       fetchTranslations('your-language-code');
   }
   ```

## 📱 响应式特性

### 断点设置
- **小屏幕**: < 576px (手机竖屏)
- **中等屏幕**: 576px - 768px (手机横屏/小平板)
- **大屏幕**: 768px - 992px (平板)
- **超大屏幕**: > 992px (桌面)

### 适配功能
- ✅ 导航栏折叠
- ✅ 自适应网格布局
- ✅ 触摸友好的按钮
- ✅ 优化的字体大小
- ✅ 弹窗自适应定位

## 🤝 贡献指南

### 开发环境设置

1. **分支管理**
   ```bash
   # 创建功能分支
   git checkout -b feature/your-feature-name
   
   # 完成开发后
   git add .
   git commit -m "feat: 添加新功能描述"
   git push origin feature/your-feature-name
   ```

2. **代码规范**
   - 使用有意义的提交信息
   - 遵循现有的代码风格
   - 添加适当的注释
   - 确保响应式兼容性

3. **测试要求**
   - 在多个设备上测试
   - 验证多语言显示
   - 检查功能完整性

### Pull Request 流程

1. Fork 本仓库
2. 创建你的功能分支
3. 提交你的更改
4. 推送到分支
5. 开启一个 Pull Request

## 📄 许可证

本项目采用 [MIT 许可证](LICENSE)。

## 🙏 致谢

- [ConcernedApe](https://twitter.com/ConcernedApe) - 《星露谷物语》游戏开发者
- [Bootstrap](https://getbootstrap.com/) - UI框架
- [jQuery](https://jquery.com/) - JavaScript库
- 所有贡献者和社区成员

## 📞 联系方式

- **Issues**: [GitHub Issues](https://github.com/Yeaowo/StardewWeb/issues)
- **Discussions**: [GitHub Discussions](https://github.com/Yeaowo/StardewWeb/discussions)

## 🔄 更新日志

### v2.0.0 (最新)
- ✨ 全新响应式UI设计
- 🌍 添加简体中文支持
- 📱 移动端优化
- 🎨 现代化界面设计

### v1.x.x
- 🎮 基础游戏功能
- 📊 数据统计功能
- 🔧 配置管理

---

**享受你的星露谷之旅！** 🌾✨
