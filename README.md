<div align="center">

# 🖼️ PicX Images Hosting

### 基于 GitHub 的免费图片托管仓库

[![GitHub stars](https://img.shields.io/github/stars/zhenttang/picx-images-hosting?style=flat-square&logo=github)](https://github.com/zhenttang/picx-images-hosting/stargazers)
[![GitHub issues](https://img.shields.io/github/issues/zhenttang/picx-images-hosting?style=flat-square&logo=github)](https://github.com/zhenttang/picx-images-hosting/issues)
[![GitHub forks](https://img.shields.io/github/forks/zhenttang/picx-images-hosting?style=flat-square&logo=github)](https://github.com/zhenttang/picx-images-hosting/network)
[![WebP](https://img.shields.io/badge/format-WebP-brightgreen?style=flat-square)](https://developers.google.com/speed/webp)
[![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)](LICENSE)

*🚀 利用 GitHub 作为免费、稳定、高速的图片 CDN 服务*

</div>

---

## 📖 项目简介

**PicX Images Hosting** 是一个基于 GitHub 仓库的静态图片托管服务，专门用于存储和分发 WebP 格式的图片资源。

本项目与 [PicX](https://github.com/XPoet/picx) 图片托管工具完美集成，利用 GitHub 作为后端存储，提供：

- 🆓 **完全免费** - 无需任何费用
- 🌍 **全球加速** - GitHub 全球 CDN 节点支持
- 🔒 **安全可靠** - GitHub 平台保障数据安全
- 📦 **无限容量** - 满足个人和小型项目需求
- 🖼️ **WebP 优化** - 更小的体积，更快的加载速度

## ✨ 核心特性

### 🎯 WebP 格式优势

- ✅ **体积更小** - 相比 PNG/JPEG 减少 25-35% 的文件大小
- ✅ **质量更高** - 在更小体积下保持优秀的视觉质量
- ✅ **加载更快** - 减少带宽消耗，提升页面加载速度
- ✅ **广泛支持** - 主流浏览器全面支持

### 🚀 GitHub 托管优势

- ✅ **版本控制** - Git 完整的版本历史记录
- ✅ **全球 CDN** - GitHub 遍布全球的 CDN 节点
- ✅ **高可用性** - GitHub 平台的高可用保障
- ✅ **免费服务** - 无需支付任何托管费用
- ✅ **API 支持** - 通过 GitHub API 和 jsDelivr CDN 加速

## 🔧 使用指南

### 方式一：使用 PicX 工具上传（推荐）

[PicX](https://github.com/XPoet/picx) 是一个简单、强大的图片托管工具，提供可视化界面：

1. 访问 [PicX 在线工具](https://picx.xpoet.cn/)
2. 使用 GitHub Token 授权登录
3. 选择本仓库 `zhenttang/picx-images-hosting`
4. 上传图片，自动转换为 WebP 格式
5. 一键复制图片外链

### 方式二：手动上传

1. **克隆仓库**
   ```bash
   git clone https://github.com/zhenttang/picx-images-hosting.git
   cd picx-images-hosting
   ```

2. **添加图片**
   ```bash
   # 将你的 WebP 图片文件复制到仓库根目录
   cp your-image.webp .
   
   # 提交并推送
   git add .
   git commit -m "Add new image"
   git push
   ```

3. **获取图片链接**
   
   上传成功后，你可以通过以下方式访问图片：

### 📎 图片链接格式

#### 🔗 GitHub 原始链接

```
https://raw.githubusercontent.com/zhenttang/picx-images-hosting/main/your-image.webp
```

#### ⚡ jsDelivr CDN 加速（推荐）

```
https://cdn.jsdelivr.net/gh/zhenttang/picx-images-hosting/your-image.webp
```

**jsDelivr 优势：**
- 🌏 全球多节点 CDN 加速
- 🚀 自动选择最快节点
- 🔄 自动缓存优化
- 🆓 完全免费

#### 📝 Markdown 格式

```markdown
![图片描述](https://cdn.jsdelivr.net/gh/zhenttang/picx-images-hosting/your-image.webp)
```

#### 🌐 HTML 格式

```html
<img src="https://cdn.jsdelivr.net/gh/zhenttang/picx-images-hosting/your-image.webp" alt="图片描述" />
```

## 📁 目录结构

本仓库采用**扁平化存储结构**，所有图片文件直接存放在根目录：

```
picx-images-hosting/
├── README.md                                    # 项目说明文档
├── image-name-1.hash.webp                       # WebP 图片文件
├── image-name-2.hash.webp                       # WebP 图片文件
└── ...                                          # 更多图片文件
```

### 📌 文件命名规范

- 图片文件名格式：`原始名称.哈希值.webp`
- 哈希值确保文件名唯一性，避免冲突
- 所有图片统一使用 WebP 格式

## 🛠️ 技术说明

### WebP 格式详解

WebP 是由 Google 开发的现代图片格式，具有以下特点：

| 特性 | 说明 |
|------|------|
| **压缩算法** | 同时支持有损和无损压缩 |
| **透明度** | 支持 Alpha 通道透明度 |
| **动画支持** | 支持动画图片（类似 GIF） |
| **元数据** | 支持 EXIF、XMP 元数据 |
| **浏览器支持** | Chrome、Firefox、Edge、Safari 等 |

### CDN 加速方案

#### 方案对比

| CDN 方案 | 速度 | 稳定性 | 推荐度 |
|----------|------|--------|--------|
| **jsDelivr** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | 🏆 强烈推荐 |
| **GitHub Raw** | ⭐⭐⭐ | ⭐⭐⭐⭐ | ✅ 可用 |

#### jsDelivr 使用技巧

```bash
# 基本格式
https://cdn.jsdelivr.net/gh/用户名/仓库名/文件路径

# 指定分支
https://cdn.jsdelivr.net/gh/用户名/仓库名@分支名/文件路径

# 指定版本
https://cdn.jsdelivr.net/gh/用户名/仓库名@版本号/文件路径

# 本仓库示例
https://cdn.jsdelivr.net/gh/zhenttang/picx-images-hosting/image.webp
```

## 📊 仓库统计

本仓库当前托管的图片资源统计：

- 📦 **图片数量**：23 张
- 🎨 **图片格式**：100% WebP
- 💾 **存储结构**：扁平化根目录存储

## 🤝 贡献指南

欢迎为本项目贡献图片资源！

### 贡献步骤

1. **Fork 本仓库**
2. **上传你的 WebP 图片**（建议通过 PicX 工具）
3. **创建 Pull Request**
4. **等待审核合并**

### 贡献要求

- ✅ 图片必须为 WebP 格式
- ✅ 确保图片内容合法合规
- ✅ 建议图片大小控制在 500KB 以内
- ✅ 使用有意义的文件名

## 📄 许可证

本项目采用 [MIT License](LICENSE) 开源协议。

## 🔗 相关链接

- 🌟 [PicX 图片托管工具](https://github.com/XPoet/picx) - 强大的图片托管管理工具
- 📚 [WebP 官方文档](https://developers.google.com/speed/webp) - Google WebP 格式说明
- ⚡ [jsDelivr CDN](https://www.jsdelivr.com/) - 免费的 CDN 加速服务
- 🐙 [GitHub Docs](https://docs.github.com/) - GitHub 官方文档

## 💬 支持与反馈

如果你在使用过程中遇到问题或有任何建议：

- 💬 [提交 Issue](https://github.com/zhenttang/picx-images-hosting/issues)
- ⭐ 如果觉得有用，请给本项目一个 Star
- 🔀 欢迎 Fork 并自定义你的图片托管仓库

---

<div align="center">

### ⭐ 如果这个项目对你有帮助，请给它一个 Star！

**Made with ❤️ by [zhenttang](https://github.com/zhenttang)**

*Powered by [PicX](https://github.com/XPoet/picx) & GitHub*

</div>
