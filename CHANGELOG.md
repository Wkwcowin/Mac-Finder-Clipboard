# 更新日志 / Changelog

## v1.0.5 (2026-03-08)

- 修复"永不超时"选项不生效的问题
- 添加文件移动成功后的通知提示
- 优化辅助功能权限检测，使用系统分布式通知实时监听权限变化，响应更及时
- 设置界面使用 0.5 秒间隔快速检测权限授予
- 改进按键模拟失败时的错误日志
- 删除未使用的代码，提高代码质量

---

## v1.0.4 (2026-1-22)

🌐 **语言选择功能 / Language Selection Feature**

### ✨ 新功能 / New Features

- 🌐 **双语支持** - 添加中文/English语言选择功能 / Added Chinese/English language selection
- 🎛️ **语言切换器** - 设置界面新增语言选择器 / New language selector in settings
- 💾 **偏好保存** - 语言选择自动保存并持久化 / Language preference auto-saved and persisted
- 🔄 **即时生效** - 切换语言后界面立即更新 / UI updates immediately after language switch
- 🌍 **智能默认** - 根据系统语言自动选择初始语言 / Auto-detect system language for initial setup

### 🎨 改进 / Improvements

- 📐 **布局优化** - 优化设置窗口布局，防止文字重叠 / Optimized settings window layout to prevent text overlap
- 🎯 **约束改进** - 改进UI约束确保各元素正确显示 / Improved UI constraints for proper element display
- 📝 **本地化** - 所有UI元素完整本地化支持 / Full localization support for all UI elements

### 🔧 技术细节 / Technical Details

- 新增 `LocalizationManager.swift` 管理多语言
- 更新所有界面组件支持动态语言切换
- 添加语言变化通知机制

---

## v1.0.1 (2024-12-09)

🎉 **首个正式发布版本**

### ✨ 功能特点

- ✂️ **真正的剪切** - 在 Finder 中使用 ⌘X 剪切文件
- 📋 **智能粘贴** - 使用 ⌘V 移动文件到目标位置
- 🎯 **场景识别** - 自动区分文件选择和文本编辑状态
- 🔔 **可视化反馈** - 剪切/粘贴操作提供清晰的通知提示
- ⏱️ **超时保护** - 可自定义超时时间（1-30分钟）
- ⚙️ **设置界面** - 精美的毛玻璃偏好设置面板
- 🚀 **开机自启** - 支持开机自动启动
- 🔄 **自动更新** - 内置 Sparkle 自动更新

### 📦 下载

- [FinderClip-1.0.1.zip](https://github.com/Wkwcowin/Mac-Finder-Clipboard/releases/download/v1.0.1/FinderClip-1.0.1.zip)

---

## v1.0.0 (2024-12-09)

🚧 内部测试版本
