# 个人站点

纯静态 HTML 网站，可直接部署到 GitHub Pages。

## 文件结构

```
/
├── index.html          # 主页
├── avatar.html         # 皮套页面
├── fanart.html        # 二创图集
├── commission.html    # 委托页面
├── character.html     # 角色设定
├── blog.html          # 个人动态
├── ip.html            # IP (占位)
├── game.html          # 游戏 (占位)
├── comic.html         # 漫画 (占位)
├── data/              # JSON 数据文件
│   ├── posts.json
│   ├── fanart.json
│   ├── price_list.json
│   ├── commission_images.json
│   └── characters.json
└── images/            # 图片文件夹
```

## 本地预览

在项目目录运行 Python 简易服务器：

```bash
python -m http.server 8080
```

然后访问 http://localhost:8080

## 部署到 GitHub Pages

1. 创建 GitHub 仓库
2. 将所有文件推送到仓库
3. 进入仓库 Settings → Pages
4. Source 选择 "Deploy from a branch"
5. Branch 选择 "main"，文件夹选择 "/ (root)"
6. 保存并等待几分钟
7. 访问 `https://你的用户名.github.io/仓库名/`

## 自定义修改

### 1. 修改首页顶部图片
编辑 `index.html`，找到：
```html
background: linear-gradient(135deg, var(--primary-color) 0%, #e8964a 100%);
```
替换为：
```html
background: url('images/top.jpg') center/cover no-repeat;
```

### 2. 修改皮套立绘
编辑 `avatar.html`，找到：
```html
<img src="images/avatar.png" alt="皮套立绘">
```
替换为你的立绘图片路径。

### 3. 修改 B 站链接
编辑 `avatar.html`，找到：
```html
<a class="bubble-btn" href="https://space.bilibili.com/" target="_blank">
```
将链接替换为你的 B 站主页链接。

### 4. 修改数据
编辑 `data/` 目录下的 JSON 文件即可动态更新内容。

## 注意事项

- 所有图片禁止右键保存已通过 `oncontextmenu="return false"` 禁用
- 响应式设计，适配手机端
- 主色调: #f7b05e (低饱和橙色)
