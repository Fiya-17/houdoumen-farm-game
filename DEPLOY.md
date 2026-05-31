# 后陡门58号：集结行动 发布说明

## 本机和同一 Wi-Fi 手机试玩

1. 在项目目录运行：

```bash
node dev-server.js
```

2. 电脑浏览器打开：

```text
http://127.0.0.1:4173/
```

3. 同一 Wi-Fi 下的手机打开：

```text
http://你的电脑局域网IP:4173/
```

当前这台电脑检测到的局域网地址是：

```text
http://192.168.3.102:4173/
```

如果手机打不开，通常是 Windows 防火墙拦截了 Node.js，需要允许 Node.js 通过专用网络。

## 发布成可分享的公网链接

推荐先用 GitHub Pages 或 Netlify 发布测试版。这个项目是纯静态网页，只需要上传整个 `houdoumen-farm-game` 文件夹，入口文件就是 `index.html`。

### GitHub Pages

1. 在 GitHub 新建公开仓库，例如 `houdoumen-farm-game`。
2. 上传 `index.html`、`dev-server.js`、`DEPLOY.md`。
3. 进入仓库 `Settings > Pages`。
4. Source 选择 `Deploy from a branch`。
5. Branch 选择 `main`，目录选择 `/root`。
6. 保存后等待 1-3 分钟，GitHub 会生成一个可分享链接。

### Netlify

1. 打开 Netlify。
2. 选择 `Add new site > Deploy manually`。
3. 把 `houdoumen-farm-game` 文件夹拖进去。
4. Netlify 会自动生成一个手机也能访问的 HTTPS 链接。

## 移动端全屏

Android Chrome 通常可以直接点击页面里的“全屏”按钮。

iPhone Safari 对网页全屏限制较多，建议用 Safari 打开链接后选择“分享 > 添加到主屏幕”，再从桌面图标进入。
