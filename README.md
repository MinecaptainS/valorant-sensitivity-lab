# 无畏契约个人灵敏度实验室

单文件网页工具：输入鼠标 DPI、当前灵敏度和个人习惯，完成内嵌的免点击甩枪、微调、跟枪测试，再比较三档灵敏度并生成建议值。测试中准星碰触目标即可命中。

## 用 GitHub Pages 发布

1. 创建一个用于此网页的 GitHub 仓库，例如 `valorant-sens-lab`。使用免费个人账号时，选择公开仓库。
2. 解压发布包，把 `index.html`、`README.md`、`.nojekyll` 上传到仓库根目录并提交到 `main` 分支；不要把它们放进额外的子文件夹。
3. 进入仓库 **Settings → Pages**，在 **Build and deployment** 中选择 **Deploy from a branch**，然后选择 **main** 和 **/(root)**，点击 **Save**。
4. 等待部署完成，打开 Pages 设置页显示的网址。项目仓库的网址通常为 `https://你的GitHub用户名.github.io/仓库名/`。

部署设置说明：[GitHub 官方文档](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)。本包不需要 npm、构建命令、Actions 工作流或服务器。

## 使用

推荐使用桌面 Chrome / Edge，开始测试时允许鼠标锁定。保持鼠标 DPI 一致，按页面提示完成九轮测评；暂停不会消耗测试时间。报告中的三位小数填入游戏「设置 → 通用 → 鼠标 → 灵敏度：瞄准」，随后在游戏靶场核验手感和保留值。

档案和报告仅存于当前浏览器的本地存储，不上传鼠标数据；离线文件与 GitHub Pages 网址的本地记录互相独立。也可以直接打开 `index.html` 离线使用。

## 来源与限制

这是独立制作的 Aim Lab 风格训练工具，并非 Riot Games 或 Aim Lab 官方产品，也未嵌入官方客户端。网页测试提供本次三档的相对表现，不能保证唯一最优灵敏度。浏览器的普通锁定、备用光标和系统加速可能影响与游戏的匹配；请优先使用原始位移路径并在游戏中核验。

模拟采用常用的 `0.07°/count × 灵敏度` 角度增益，16:9 下水平视场角为 103°；网页中列有完整说明与公式。主要资料：

- [Riot 11.06 更新：原始输入始终启用](https://playvalorant.com/en-us/news/game-updates/valorant-patch-notes-11-06/)
- [Riot 13.09 更新](https://playvalorant.com/en-us/news/game-updates/valorant-patch-notes-1309/)
- [KovaaK 开发者补丁说明：0.07 匹配参数](https://www.reddit.com/r/FPSAimTrainer/comments/gg4iu1/2010_patch_notes/)
- [Aimlabs 官方灵敏度配置教程](https://aimlabs.com/articles/aimlabs/how-to-configure-and-convert-your-sensitivity-in-aimlabs/)

资料核查日期：2026-11-03。请以安装的游戏客户端最终接受与保留的数值为准。
