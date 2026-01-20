<div align="center">
  <!-- 标题区域：Flex/Table 混合布局确保垂直居中 -->
  <table style="border: none; background: none;">
    <tr style="border: none; background: none;">
      <td style="border: none; background: none; padding: 0; vertical-align: middle;">
        <img src="https://x19.fp.ps.netease.com/file/696c8a128f0376b4ef2ee155d5ZmuGRq07" width="64" height="64" style="border-radius: 12px;" />
      </td>
      <td style="border: none; background: none; padding-left: 15px; vertical-align: middle;">
        <h1 style="margin: 0; font-size: 42px; border-bottom: none;">Hypixice Music</h1>
      </td>
    </tr>
  </table>

  <!-- 徽章区域 -->
  <p style="margin-top: 10px;">
    <img src="https://img.shields.io/badge/Version-1.1.6-blue?style=flat-square" alt="Version">
    <img src="https://img.shields.io/badge/Status-Beta-orange?style=flat-square" alt="Status">
    <img src="https://img.shields.io/badge/License-Proprietary-red?style=flat-square" alt="License">
  </p>

  <p>
    <strong>一款基于网易云音乐的轻量级一站式网页播放器</strong><br>
    支持逐字歌词 · 沉浸式背景 · 多源API解析 · 无损下载
  </p>

  <p>
    <a href="https://www.hypixice.top/tw/h-music"><strong>🌐 在线体验 (Web版)</strong></a> | 
    <a href="https://status.hypixice.top/"><strong>📊 服务状态页</strong></a> |
    <a href="https://gitee.com/Hypixice_master/hypixice-music/releases/"><strong>⬇️ 下载离线版</strong></a>
  </p>
</div>

---

<!-- 截图展示区域 -->
<div align="center">
  <h3>📱 软件预览</h3>
  <table style="border: none;">
    <tr>
      <td align="center" style="border: none; padding: 10px;">
        <img src="https://x19.fp.ps.netease.com/file/696c8e512d5a176d701727daAr9rU0UO07" alt="主界面" width="400" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);" />
        <br><sub>🎵 沉浸式播放界面</sub>
      </td>
      <td align="center" style="border: none; padding: 10px;">
        <img src="https://x19.fp.ps.netease.com/file/696c8b82092c363c50226389PffwoZtx07" alt="搜查页" width="400" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);" />
        <br><sub>🔍 全新搜查与下载页</sub>
      </td>
    </tr>
  </table>
</div>

---

## 📌 简介

**Hypixice Music** 是由 [HYPIXICE 工作室](https://www.hypixice.top/) 开发的一款仿 **Apple Music** 风格的网易云音乐播放器。

它不仅支持解析网易云音乐分享链接，最新版本还内置了**歌曲搜索**功能。项目由 TurboWarp 驱动，提供极致的本地化播放与歌词同步体验，支持将带有**元数据（封面/专辑信息）**的音频文件下载到本地。

> ⚠️ **注意**：本项目目前**暂不开源**，仅发布编译后的使用版本。

---

## ✨ 核心功能 (v1.1.6 新增)

根据最新更新，播放器现已支持以下特性：

- **🛡️ 多源 API 保障**：新增 `haitangw` 等多源 API 插件支持。当首选接口拉取失败时，自动切换至备用接口，大幅提升可用性。
- **🔊 全新音量 UI**：重构了音量控制界面，支持更精细的调节与悬浮提示。
- **🔍 极速搜查**：支持在搜查页直接按下 **回车键 (Enter)** 发起搜索，交互更顺滑。
- **💾 高级下载**：支持 **FLAC 无损** 及 MP3 格式下载，自动写入完整元数据（封面/歌手/专辑）。
- **📉 状态反馈**：新增进度条错误状态显示，拉取失败一目了然。

---

## 🛠 技术细节

### 歌词来源
- **逐字歌词**：基于 AMLL 抓包 API 实现精准卡点。
- **普通歌词**：直接获取网易云 API，并通过 AerMini 拓展转换为 TTML 格式。

### 技术架构
- **运行环境**：纯前端网页应用（无需后端）。
- **核心引擎**：[TurboWarp](https://turbowarp.org/)（基于 Scratch 的高性能运行时）。
- **开发语言**：JavaScript + HTML。

---

## 🚀 使用方法

### 方式一：网页版（推荐）
直接访问 **[在线体验地址](https://www.hypixice.top/tw/h-music)** 即可使用最新功能。

### 方式二：离线版（本地运行）
1. 前往 **[Releases 页面](https://gitee.com/Hypixice_master/hypixice-music/releases/)** 下载最新版 `.html` 文件。
2. 双击在浏览器中打开该文件。

### 🕹️ 操作指南
- **搜索歌曲**：输入歌名后按 **Enter 键** 或点击按钮查找。
- **链接解析**：按下键盘 **`P` 键**，粘贴网易云音乐的歌曲/歌单分享链接。
- **音量调节**：悬停音量图标唤出全新 UI，使用滚轮或拖动调节。
- **下载**：在播放或搜索界面点击下载按钮，支持选择音质。

---

## ⚠️ 已知问题

- **API 维护**：网易云音乐 API 通常在**凌晨时段进行维护**。虽然加入了多源支持，但仍可能偶发不稳定。
- **兼容性**：部分低端设备或旧版浏览器可能无法正确渲染模糊/光晕效果。

---

## 📝 更新日志

### **Beta_Release_1.1.6 (Latest)**
> 交互体验优化与稳定性提升
- **[新增]** 新增 API 插件 `haitangw`，扩充解析源。
- **[新增]** 完整的音量操作 UI 面板。
- **[新增]** 界面按钮增加操作悬浮提示 (Tooltip)。
- **[新增]** 搜查页面支持 **回车键 (Enter)** 确认搜索。
- **[修复]** 拉取失败时进度条显示红色错误状态。
- **[优化]** 优化整体 UI 细节设计。

### **Beta_Release_1.1.5-fix2**
> 多源容灾与细节修复
- **[新增]** **多源 API 系统**：首个 API 失败时自动尝试备用源。
- **[新增]** 进度条增加错误状态逻辑。
- **[修复]** 修复下载歌词按钮失效的问题。
- **[修复]** 修复了大量细节 Bug。
- **[优化]** 优化页面视觉设计。

### **Beta_Release_1.1.4-fix1**
> 无损音频与搜查下载
- **[新增]** 支持 FLAC 无损音频写入。
- **[新增]** 搜查页面支持直接下载音频。
- **[修复]** 修复加载动画断裂及遮罩显示问题。
- **[修复]** 修复解析音频音质不匹配的问题。

---

## 📬 反馈与交流

虽然本项目暂不开源，但我们非常欢迎您的反馈！
如果您在使用过程中遇到 Bug 或有功能建议：

1. 请查看 **[服务状态页](https://status.hypixice.top/)** 确认是否为服务器问题。
2. 在仓库的 **Issues** 页面提交反馈。

---

## 🙏 特别感谢

- **AerMini**：提供转换扩展模块支持。
- **ciallo**：提供 FLAC/MP3 音频处理下载器。
- **mecll**：提供网易云音乐拓展支持。
- **Cyberexplorer**：提供拓展支持。
- **[看戏仔](https://api.kxzjoker.cn/)**：提供网易云解析服务支持。

---

<div align="center">
    Made with ❤️ b
