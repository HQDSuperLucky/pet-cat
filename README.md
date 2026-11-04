# 今天也要摸摸猫

手机和电脑浏览器均可游玩的轻量 H5 猫咪互动游戏。

## 玩法

点击或滑动猫咪进行抚摸，使用喂食和逗猫按钮获得好感。
好感达到 30、80、150 时解锁收藏。每天互动 10 次获得额外 15 点好感。
小鱼干每分钟补充 1 条，上限为 5 条。
进度保存在当前浏览器本地，不跨设备同步。

## 部署到 GitHub Pages

1. 将此目录全部文件（包括 `.github/workflows/pages.yml`）提交到仓库的 `main` 分支。
2. 在仓库 Settings → Pages → Build and deployment 中，将 Source 设为 GitHub Actions。
3. 在 Actions 中运行 Publish cat game to GitHub Pages，或再次提交修改触发部署。
4. 等待部署成功，访问 Pages 显示的网站地址。

游戏无需安装依赖或执行构建。所有资源使用相对路径，适用于 GitHub Pages 的项目子路径。
也可以选择 Deploy from a branch，指定 main 分支和根目录，以无需 Actions 的方式发布。

## 本地运行

在此目录运行 `python -m http.server 8765`，再访问 http://localhost:8765。
