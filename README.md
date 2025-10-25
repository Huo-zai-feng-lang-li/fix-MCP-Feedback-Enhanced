# MCP Feedback Enhanced

## 🔧 本地定制版本说明

> 感谢原作者的反馈项目，本版本修复了以下问题并新增功能：

### ✅ 已修复问题

1. **超时设置问题**：修复了超时时间永远是 600s 的问题，现已修复默认 24 小时超时
   ，可以长时间等待反馈啦
2. **图片上传问题**：修复了无法上传图片报错序列号错误的问题，现已支持更多类型图
   片 😁🎉
3. **断网重连功能**：新增断网不断链接功能，现在可以离线同一个会话等待（适合使用
   手机热点为电脑提供互联网的场景）

### 🚀 如何使用

Fork 本项目到本地，在 Cursor 中配置：

```json
{
  "mcpServers": {
    "mcp-feedback-enhanced-local": {
      "command": "uv",
      "args": [
        "run",
        "--directory",
        "C:\\Users\\Administrator\\Desktop\\project\\mcp-feedback-enhanced-main",
        "python",
        "-m",
        "mcp_feedback_enhanced"
      ],
      "timeout": 86400,
      "env": {
        "MCP_DEBUG": "false",
        "MCP_WEB_HOST": "127.0.0.1",
        "MCP_WEB_PORT": "8765",
        "MCP_DESKTOP_MODE": "false",
        "MCP_LANGUAGE": "zh-CN"
      },
      "autoApprove": ["interactive_feedback"]
    }
  }
}
```

> **注意**：请将
> `"C:\\Users\\Administrator\\Desktop\\project\\mcp-feedback-enhanced-main"` 改
> 为您本地的项目位置，这样可以实现本地高自由度的定制。

### 📸 界面预览

<div align="center">
  <img src="images/0.png" width="600" alt="MCP Feedback Enhanced 界面预览" />
  <br>
  <em>主界面 - 支持提示管理、自动提交、会话跟踪上传图片等功能</em>
</div>

<div align="center">
  <img src="images/1.png" width="600" alt="MCP Feedback Enhanced 功能展示" />
  <br>
  <em>超时功能展示 - 智能工作流程和现代化体验</em>
</div>

---

**🌐 Language / 語言切換:** **English** | [繁體中文](README.zh-TW.md) |
[简体中文](README.zh-CN.md)
