# song-jinghao.github.io

Song Jinghao 的 GitHub Pages 个人主页初版。

在线地址：

```text
https://song-jinghao.github.io/
```

## 目录结构

```text
song-jinghao.github.io/
├─ index.html
├─ README.md
├─ .nojekyll
└─ assets/
   ├─ css/
   │  └─ style.css
   ├─ js/
   │  └─ main.js
   └─ images/
      └─ avatar.svg
```

## 第一次上传

如果你的仓库已经创建好，并且本地还没有拉取：

```bash
git clone https://github.com/song-jinghao/song-jinghao.github.io.git
cd song-jinghao.github.io
```

把本压缩包中的文件复制到仓库根目录，然后：

```bash
git add .
git commit -m "init personal homepage"
git push origin main
```

## GitHub Pages 设置

一般 `用户名.github.io` 仓库会自动作为个人 Pages 站点使用。

如果没有上线：

1. 打开 GitHub 仓库。
2. `Settings` → `Pages`
3. `Build and deployment`
4. Source 选择 `Deploy from a branch`
5. Branch 选择 `main`
6. Folder 选择 `/ (root)`
7. 保存。

稍后访问：

```text
https://song-jinghao.github.io/
```

## 后续怎么修改个人信息

最常改的是：

```text
index.html
```

在编辑器里全局搜索：

```text
TODO
请修改
待填写
请核对
```

就可以快速找到所有需要替换的位置。

### 替换头像

把你的头像放到：

```text
assets/images/avatar.jpg
```

然后在 `index.html` 搜索：

```html
src="assets/images/avatar.svg"
```

改成：

```html
src="assets/images/avatar.jpg"
```

同时建议把 `og:image` 也从 `avatar.svg` 改为 `avatar.jpg`。

## 本地预览

在项目根目录执行：

```bash
python -m http.server 8000
```

浏览器打开：

```text
http://localhost:8000
```

## 风格

整体采用简洁的学术 / 技术简历布局：

- 顶部固定导航
- 左侧个人信息
- 右侧经历与项目
- 白灰背景 + 红色强调色
- PC / 手机响应式适配
- 手机端折叠菜单
- 当前章节导航高亮

后续可以继续增加：

- 中英文切换
- 深色模式
- Publications / Blog
- GitHub 项目卡片
- PDF 简历下载
- Codeforces / LeetCode 信息
- Google Analytics
