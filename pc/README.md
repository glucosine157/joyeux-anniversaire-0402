# 完整 PC 版生日网页上传包

这是完整电脑端版本，不是移动端精简页。

## 必需文件

- `index.html`
- `campus-data.js`
- `sjtu-emblem-white.svg`
- `.nojekyll`

## 这版的特点

- 保留完整的 PC 端视觉效果
- 保留摄像头和手势识别逻辑
- 保留三屏滚动和粒子动画
- 适合桌面浏览器访问

## 上传到 GitHub 仓库时

把这个文件夹里的内容直接放到仓库根目录。

不要只上传 `index.html`，另外两个资源文件也必须一起上传。

## GitHub Pages 设置

仓库里不需要 `yml` 也能部署。

在 GitHub 仓库里这样设置：

1. `Settings`
2. `Pages`
3. `Source` 选 `Deploy from a branch`
4. `Branch` 选 `main`
5. `Folder` 选 `/(root)`
6. `Save`

## 部署后注意

- 第一次生效通常要等 1 到 3 分钟
- 页面需要 `HTTPS`
- 摄像头手势识别需要用户允许浏览器摄像头权限
- 建议用桌面版 Chrome 或 Safari 打开

## 说明

虽然它是“完整动态网页”，但部署形式仍然是前端静态托管：

- 动画、Three.js、手势识别都在浏览器里运行
- 不需要后端服务器

所以 GitHub Pages、Vercel、Netlify 都能托管这版
