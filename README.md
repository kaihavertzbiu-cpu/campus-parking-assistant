# Campus Parking Assistant / 校园停车助手

Cornell 校园停车决策展示原型：比较停车地点、费用与步行距离，提供地图查看、方案对比和收藏。

![界面预览](docs/preview.png)

## 项目范围

本版本基于 Team 24 的 SYSEN 5151 课程项目，保留页面中的来源与个人贡献说明。车位与需求情景使用模拟数据，不是校园实时停车服务，也没有接入停车收费或真实预订。

`index.html` 内含页面样式、交互逻辑和必要图像。收藏等本地状态由浏览器保存；不同设备不会自动同步。独立包的品牌链接改为返回当前页面，不依赖个人主页。

## GitHub Pages / Netlify

纯静态页面，无需安装前端依赖。双击 index.html，或在仓库根目录运行 `python -m http.server 8000` 后打开 http://localhost:8000/。

GitHub 仓库 Settings → Pages → Deploy from a branch，选择 main 与 /(root)。说明依据：[GitHub 官方发布文档](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)。根目录 .nojekyll 用于保留静态站点。

Netlify 手动部署时上传站点文件；首页 index.html 位于根目录。README 与源码不会自动替你完成线上发布。

## 上传 GitHub

解压本项目的 ZIP。把解压后的文件和目录作为仓库内容上传，README.md 应在仓库根目录；不要只上传 ZIP 本身。项目之间分别建仓库。

也可以在解压目录打开终端执行（将 REPOSITORY_URL 替换成自己的 GitHub 仓库地址）：

```sh
git init
git add .
git commit -m "Initial project source"
git branch -M main
git remote add origin REPOSITORY_URL
git push -u origin main
```

这些步骤需要你自己的 GitHub 账号和仓库；本包没有账号令牌或自动发布脚本。
