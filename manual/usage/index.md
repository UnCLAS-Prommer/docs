# MaiBot 使用指南

本章节将介绍 MaiBot 的日常使用方法、常见问题解答和最佳实践，帮助您更好地使用和管理机器人。

## 基本使用

MaiBot 设计为通过自然对话方式与用户交互，只需在群内@机器人或发送私聊消息，即可开始对话。

### 唤醒方式

- 在群聊中@机器人（推荐）
- 在群聊中发送机器人的名字（配置文件中设置的名称）
- 直接私聊机器人

### 基础功能

- **自然对话**：与机器人进行自然语言对话
- **表情包收集**：机器人会自动收集群内分享的表情包
- **知识库查询**：机器人可以回答关于预设知识库的问题

## 配置调整

如需调整机器人的行为，请修改配置文件而非通过聊天命令。主要配置文件：

- `bot_config.toml` - 机器人行为配置
- `.env` - 环境和API配置

修改配置后，需要重启机器人使更改生效。

## 常见问题解答

有关常见问题的详细解答，请参考[快速问答](./fast_q_a)页面，其中包含：

- API 相关问题
- MongoDB 相关问题
- 部署故障排除
- 功能使用疑问

## 最佳实践

### 对话技巧

- 使用清晰、简洁的语言
- 一次提问专注于一个主题
- 如需连续对话，请保持在同一话题上下文中

### 性能优化

- 定期清理数据库中的表情包和不必要数据
- 使用较长的对话记忆窗口会增加API消耗
- 多个机器人共享同一数据库可能导致性能下降

### 安全建议

- 尽量不要暴露相应服务端口到公网
- 使用专用的小号作为机器人账号
- 定期更新API密钥
- 不要在机器人配置中存储敏感信息
- 保持服务器和依赖项的更新
