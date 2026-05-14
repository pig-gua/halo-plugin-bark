## 🏗️ 技术架构

### 后端组件

- **BarkService**: 核心服务类，负责处理 Bark 推送逻辑
- **CommentReconciler**: 评论监听器，检测新评论并触发通知
- **RegisterReconciler**: 用户注册监听器，检测新用户并触发通知
- **BarkEndpoint**: API 接口，提供推送测试功能

### 前端技术栈

- Vue 3 + TypeScript
- Rsbuild 构建工具
- Element Plus UI 组件库

### 工作流程

1. 插件监听 Halo 系统中的评论和用户注册事件
2. 当事件发生时，检查是否已处理过该事件（避免重复通知）
3. 根据用户配置生成 Bark 推送请求
4. 向指定的 Bark 服务器发送 HTTP 请求
5. 用户 iOS 设备接收到推送通知

## 📱 Bark 应用使用

1. 在 IOS App Store 下载并安装 [Bark](https://apps.apple.com/app/bark-customed-notifications/id1403753865)
2. 打开应用获取设备 Key
3. 将设备 Key 填入插件配置中
4. 可选：部署自己的 Bark 服务器以获得更好的隐私保护

## 🤝 贡献指南

欢迎提交 Issue 和 Pull Request 来改进这个插件：

1. Fork 本仓库
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启 Pull Request

## 📄 许可证

本项目采用 GPL-3.0 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情

## 👨‍💻 作者

- **呱仔** - [Pig-Gua](https://github.com/pig-gua)
- 网站: [https://abaaba.cloud](https://abaaba.cloud)

## 🙏 致谢

- [Halo](https://halo.run) - 优秀的开源博客系统
- [Bark](https://bark.day.app/) - 强大的 iOS 推送服务
- 所有为这个项目做出贡献的开发者们

---

如果这个项目对您有帮助，请考虑给它一个 ⭐️ Star！
