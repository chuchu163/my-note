# Markdown 内容展示

一个简单的Markdown内容展示和编辑网页，支持本地存储和GitHub Pages部署。

## 功能特点

- 📝 主界面显示Markdown渲染后的内容
- 📁 支持导入Markdown或文本文件
- ✏️ 支持在线编辑内容
- 💾 内容自动保存到浏览器本地存储
- 🌐 可通过GitHub Pages部署访问

## 本地使用

1. 直接在浏览器中打开 `index.html` 文件即可使用
2. 内容会保存在浏览器的localStorage中

## GitHub Pages 部署步骤

### 方法一：使用GitHub网页界面

1. 在GitHub上创建一个新的仓库
2. 将 `index.html` 文件上传到仓库
3. 进入仓库的 **Settings**（设置）
4. 在左侧菜单中找到 **Pages**
5. 在 **Build and deployment** 部分：
   - **Source** 选择 `Deploy from a branch`
   - **Branch** 选择 `main` 或 `master` 分支，文件夹选择 `/ (root)`
6. 点击 **Save**
7. 等待几分钟，网站就会部署完成
8. 访问地址格式为：`https://你的用户名.github.io/仓库名/`

### 方法二：使用Git命令行

1. 在GitHub上创建一个新的仓库
2. 在本地项目目录中打开终端，执行以下命令：

```bash
git init
git add index.html README.md
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/你的用户名/仓库名.git
git push -u origin main
```

3. 然后按照方法一的步骤3-8配置GitHub Pages

## 注意事项

- 内容保存在浏览器的localStorage中，清除浏览器数据会丢失内容
- 不同设备或浏览器之间的内容不会同步
- 如果需要跨设备同步，可以考虑使用GitHub Gist或其他云存储服务

## 技术栈

- HTML5
- CSS3
- JavaScript
- [Marked.js](https://marked.js.org/) - Markdown解析库
