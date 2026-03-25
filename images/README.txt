# 图片存放说明

此文件夹用于存放所有静态图片。

## 首页轮播图（必需）
- `top1.jpg` - 轮播图第1张
- `top2.jpg` - 轮播图第2张
- `top3.jpg` - 轮播图第3张

## 皮套页面
- `avatar.png` - 皮套立绘（大图PNG，无边框）

## 二创图集 (fanart)
- `fanart1.jpg` ~ `fanart6.jpg`

## 委托展示
- `commission1.jpg` ~ `commission6.jpg`

## 博客配图
- `post1.jpg`, `post2.jpg` 等（根据博客内容添加）

## 角色图鉴（PNG格式，无边框）
- 缩略图：`thumb_a.png` ~ `thumb_j.png`（建议 200x200 圆形区域）
- 详情图（三张）：`detail_a1.png`, `detail_a2.png`, `detail_a3.png` 等

## 官方二创页面
### 角色头像（必需）
- `official/avatar_a.png` - 角色A头像
- `official/avatar_b.png` - 角色B头像
- `official/avatar_c.png` - 角色C头像
- 可按需添加更多角色头像

### 角色图集（可选，数量不限）
每个角色的图集放在 `official/` 目录下：
- `a_gallery1.jpg`, `a_gallery2.jpg`, `a_gallery3.jpg` - 角色A的图集
- `b_gallery1.jpg`, `b_gallery2.jpg` - 角色B的图集
- 以此类推...

### JSON数据配置
编辑 `data/official_fanart.json` 动态配置角色和图集：
```json
{
  "name": "角色名称",
  "avatarUrl": "images/official/avatar_xxx.png",
  "gallery": [
    { "imageUrl": "图片路径", "caption": "注释文字" },
    { "imageUrl": "图片路径", "caption": "注释文字" }
  ]
}
```

## 图片尺寸建议

- 首页轮播: 1920x1080 或 16:9
- 立绘: 宽800px以上，高度自适配
- 博客图片: 800x600 或等比例
- 角色缩略图: 200x200 正方形
- 角色头像（官方二创）: 200x200 圆形
- 角色详情图: 800x1000 或等比例
- 官方二创图集: 800x1000 或等比例
