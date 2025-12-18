# 魔方教学视频平台 | Rubik's Cube Tutorial Video Platform

一个基于网页的魔方教学视频平台，包含F2L、OLL和PLL解法的图解和视频教程。

A web-based Rubik's cube tutorial video platform featuring visual guides and video tutorials for F2L, OLL, and PLL solutions.

## 功能特点 | Features

- 🧩 **完整的解法库**: 包含F2L (41个)、OLL (57个)、PLL (21个)解法
- 📹 **视频教程**: 每个解法都配有B站教学视频
- 🖼️ **图解展示**: 直观的解法图解帮助理解
- 📝 **统一选择框架**: 在同一个选择框内完成解法类型和具体解法的选择
- 📱 **响应式设计**: 支持桌面和移动设备
- ⌨️ **键盘导航**: 支持方向键快速浏览解法

## 项目结构 | Project Structure

```
cube/
├── index.html              # 主页面 (包含所有解法数据和JavaScript代码)
├── style.css              # 样式文件
├── images/                # 解法图片目录
│   ├── image_F2L_001.bmp  # F2L解法图片
│   ├── image_OLL_001.bmp  # OLL解法图片
│   └── image_PLL_001.bmp  # PLL解法图片
├── wrangler.toml          # Cloudflare Pages配置
├── README.md              # 项目说明文档
└── docs/                  # 文档目录 (可选)
```


## 本地运行 | Local Development

### 方法1: 使用Python简单服务器

```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

然后访问 `http://localhost:8000`

### 方法2: 使用Node.js服务器

```bash
# 安装http-server
npm install -g http-server

# 运行服务器
http-server -p 8000
```

### 方法3: 使用VS Code Live Server

1. 安装 Live Server 扩展
2. 右击 `index.html` 选择 "Open with Live Server"

## 部署到Cloudflare Pages | Deploy to Cloudflare Pages

### 方法1：GitHub集成部署 (推荐)

1. **创建Pages项目**
   - 登录 [Cloudflare Dashboard](https://dash.cloudflare.com/)
   - 转到 "Pages" 页面
   - 点击 "Create a project"
   - 选择 "Connect to Git"

2. **连接GitHub仓库**
   - 选择你的GitHub仓库
   - 设置构建配置：
     - **Framework preset**: None (Static HTML)
     - **Build command**: (留空)
     - **Build output directory**: /
   - 点击 "Save and Deploy"

### 方法2：直接上传部署

1. **准备文件**
   - 确保所有文件在项目根目录
   - 主要文件：`index.html`, `style.css`, `images/` 文件夹

2. **直接上传**
   - 在 Cloudflare Pages 中选择 "Upload assets"
   - 拖拽整个项目文件夹或上传 ZIP 文件
   - 自动部署完成

## 解法数据 | Solution Data

- **F2L**: 41个基础F2L情况
- **OLL**: 57个OLL解法 (包含所有情况)
- **PLL**: 21个PLL解法 (包含所有排列)

每个解法都包含：
- 图解展示
- 详细步骤
- 教学视频链接

## 贡献指南 | Contributing

1. Fork 本项目
2. 创建特性分支: `git checkout -b feature/AmazingFeature`
3. 提交更改: `git commit -m 'Add some AmazingFeature'`
4. 推送到分支: `git push origin feature/AmazingFeature`
5. 提交Pull Request

## 许可证 | License

本项目采用 GPLv3 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情。

## 联系方式 | Contact

如果您有任何问题或建议，请通过以下方式联系：

- 创建 [Issue](https://github.com/liuhangbin/cube/issues)

## 致谢 | Acknowledgments

- 感谢魔方吧社区提供的资源
- 感谢Cloudflare提供的免费部署平台

---

⭐ 如果这个项目对您有帮助，请给我们一个星标！

⭐ If this project helps you, please give us a star!
