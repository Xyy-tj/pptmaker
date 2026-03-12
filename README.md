# PPTMaker (EvilPPT)

🚀 **基于 HTML 的智能 PPT 生成与演示工具**

PPTMaker 是一个基于 Electron 开发的桌面应用程序，旨在通过 AI 技术帮助用户快速生成高质量的 HTML 演示文稿。它结合了现代 Web 技术的灵活性和 AI 的创造力，让演示文稿的制作变得简单而高效。

## ✨ 主要特性

*   **🤖 智能生成**：集成 OpenAI/Gemini/Claude 等先进大模型，一键生成演示大纲与内容。
*   **📊 项目管理**：直观的仪表盘，轻松管理多个演示项目。
*   **👁️ 实时预览**：内置演示播放器，所见即所得。
*   **🎨 HTML 幻灯片**：基于 Web 技术构建，支持丰富的 CSS 动画与交互。
*   **⚙️ 灵活配置**：支持自定义 API Endpoint、模型选择（GPT-5.4, Gemini-3-Pro 等）及系统提示词。

## 📥 快速安装 (Release 版本)

如果您不需要修改源码，推荐直接下载我们编译好的安装包，这是最快的使用方式：

1.  访问本项目的 [**Releases 页面**](https://github.com/Xyy-tj/pptmaker-html/releases)。
2.  找到最新版本（Latest），下载对应的安装包：
    *   **Windows**: 下载 `.exe` 文件 (如 `PPTMaker Setup 1.0.0.exe`)
    *   **macOS/Linux**: (如果有提供) 下载对应的 `.dmg` 或 `.AppImage`
3.  双击下载的安装包，按照提示完成安装。
4.  安装完成后，即可在桌面或应用列表中启动 **PPTMaker**。

## ⚙️ 初次使用配置

启动应用后，为了使用 AI 智能生成功能，您需要进行简单的配置：

1.  点击左侧侧边栏底部的 **"系统设置" (Settings)**。
2.  **API Key**: 输入您的 API 密钥（支持 OpenAI 格式或兼容的 API Key）。
3.  **Base URL**: (可选) 如果您使用官方接口可留空；如果使用中转服务，请输入完整的 Base URL (例如 `https://api.openai.com/v1`)。
4.  **模型选择**: 选择您偏好的模型 (如 `gemini-3-pro-preview`, `gpt-4` 等)，也支持手动输入自定义模型名称。
5.  点击 **"测试连通性"** 按钮验证配置是否正确。
6.  验证通过后，点击 **"保存配置"**。

## 🛠️ 开发指南

如果您是开发者，想要贡献代码或进行二次开发，请按以下步骤操作：

### 环境要求

*   **Node.js**: 建议 v16 或更高版本
*   **npm** 或 **yarn**

### 1. 获取源码

```bash
git clone https://github.com/Xyy-tj/pptmaker-html.git
cd pptmaker-html
```

### 2. 安装依赖

```bash
npm install
```

### 3. 启动开发模式

```bash
npm start
```

### 4. 构建安装包

如果您想自己编译 Release 版本：

```bash
# 构建 Windows 安装包 (生成的安装包位于 dist 目录)
npm run dist
```

## 📂 项目结构

*   `main.js`: Electron 主进程入口文件。
*   `index.html`: 应用的主界面入口。
*   `assets/`: 包含样式 (CSS) 和前端逻辑 (JS)。
*   `slides/`: 存放生成的幻灯片 HTML 文件，每个项目一个文件夹。
*   `projects.json`: 用于存储项目列表和元数据的 JSON 文件。

## 📄 许可证

本项目采用 [ISC License](LICENSE) 授权。
