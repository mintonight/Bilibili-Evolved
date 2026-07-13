# 独立油猴脚本

不依赖 [Bilibili Evolved](https://github.com/the1812/Bilibili-Evolved)，单独安装即可使用。

## B站仅搜索首页

文件：[`bilibili-search-only-home.user.js`](./bilibili-search-only-home.user.js)

### 功能

- 仅在 `www.bilibili.com` 首页生效
- 隐藏推荐流、频道栏、横幅装饰
- **保留顶栏**（消息、头像等）
- 页面中央大搜索框
- 默认**纯黑**背景
- 支持菜单修改背景颜色 / 背景图
- 输入 `BV…` / `av…` / 纯数字可尝试直达视频页

### 安装

1. 浏览器安装 [Tampermonkey](https://www.tampermonkey.net/)（或 Violentmonkey 等）
2. 打开下面任一安装链接，油猴会提示安装：

**jsDelivr（推荐）：**

```text
https://cdn.jsdelivr.net/gh/mintonight/Bilibili-Evolved@feature/search-home/userscripts/bilibili-search-only-home.user.js
```

**GitHub Raw：**

```text
https://raw.githubusercontent.com/mintonight/Bilibili-Evolved/feature/search-home/userscripts/bilibili-search-only-home.user.js
```

3. 打开 [https://www.bilibili.com/](https://www.bilibili.com/) 即可

### 设置背景

在油猴扩展图标 → 本脚本的菜单命令：

| 菜单 | 作用 |
|------|------|
| 设置背景颜色 | 例如 `#000000`、`#111`、`rgb(0,0,0)` |
| 设置背景图片 URL | `https://...` 图片地址，留空清除 |
| 恢复默认背景 | 恢复纯黑 |

### 与 Evolved 组件版区别

| | 油猴独立脚本 | Evolved 组件「仅搜索首页」 |
|--|-------------|---------------------------|
| 依赖 | 仅油猴 | 需要 Bilibili Evolved |
| 搜索框 | 自带简单搜索 | 脚本 LaunchBar（可接搜索插件） |
| 安装 | 点脚本链接安装 | Evolved 内装组件 JS |

两者不要同时开，以免重复隐藏、叠两层搜索框。

### 源码

- 脚本：`userscripts/bilibili-search-only-home.user.js`
- Evolved 组件源码：`registry/lib/components/style/home-redesign/search/`
