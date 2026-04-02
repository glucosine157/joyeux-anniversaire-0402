# NFC 移动版生日页

这个版本是为 `手机浏览器 + NFC` 重做的单页：

- 不依赖摄像头
- 不依赖 Three.js / MediaPipe
- 适合手机打开
- 可直接部署到任意静态托管

## 文件

- `index.html`
- `sjtu-emblem-white.svg`

## 本地预览

直接双击 `index.html` 即可。

如果你想模拟上线环境，也可以在这个目录执行：

```bash
python3 -m http.server 8000
```

然后打开：

```text
http://localhost:8000
```

## 上线方式

把整个文件夹上传到任意静态托管即可，例如：

- Vercel
- Netlify
- GitHub Pages
- Cloudflare Pages

## NFC 正确写法

不要把 HTML 写进 NFC 卡。

正确做法是：

1. 先把这个页面部署成 `HTTPS` 链接
2. 把这个链接写进 NFC 卡
3. 手机碰卡后直接打开这个页面

## 建议

如果这个链接主要给手机打开，建议使用：

- 短链接
- HTTPS
- 不要再加需要登录或下载 App 的跳转
