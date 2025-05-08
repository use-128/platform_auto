# 各大平台自动发布系统

## 小红书

社交媒体自动化专家开发的 **小红书自动发布脚本系统**，支持模块化管理、定时发布、内容队列处理，并支持未来扩展如微博、抖音等平台。以合规、安全、高效为核心设计理念。

---

🚀 快速开始
初始化 .env 文件并填写敏感信息：

ENCRYPT_SECRET_KEY=your_32byte_key_here
EMAIL_PASSWORD=your_email_password
WEIBO_ACCESS_TOKEN=weibo_token_example
编辑 config/settings.yaml 配置内容和账号信息。

启动主程序：
```bash
python main.py
```

🛠 功能模块
✅ 小红书模块（xiaohongshu）
使用 DrissionPage 控制浏览器

自动填写图文、发布内容

加载图文素材队列

支持定时调度、异常重试、发布监控

✅ 配置与安全
所有行为参数通过 settings.yaml 管理

敏感参数通过 .env 管理并忽略 Git 提交

模块间解耦、支持多平台扩展

📡 未来扩展
✅ 微博平台模块（已预留结构）

⏳ 抖音发布支持

✅ 多账号轮换处理

✅ Slack / 钉钉 推送通知

📊 Web控制面板与可视化统计

📄 开发须知
项目遵循模块化 + 可扩展架构，每个平台独立文件夹。

推荐使用 venv 进行隔离环境管理。

本项目仅限合规使用，请勿用于违反平台协议的自动行为。

📬 联系与支持
作者：lzb
版本：0.1
