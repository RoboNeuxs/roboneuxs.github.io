# 发布到 roboNeuxs 组织

目标仓库：https://github.com/roboNeuxs/roboneuxs.github.io
发布后的网页：https://roboneuxs.github.io/

1. 打开 https://github.com/new。Owner 选择 roboNeuxs；仓库名填写 roboneuxs.github.io（全部小写）；选择 Public，并勾选 Add README，然后创建仓库。
2. 解压 roboneuxs-pages.zip。在仓库 main 分支点击 Add file → Upload files，上传 index.html、clock.html、sensor-experiments.zip 和 .nojekyll，点击 Commit changes 提交到 main。
3. 打开仓库 Settings → Pages。在 Build and deployment 中，Source 选择 Deploy from a branch，Branch 选择 main，文件夹选择 /(root)，点击 Save。
4. 等待 Pages 发布成功，再访问 https://roboneuxs.github.io/。Settings → Pages 的 Visit site 可以打开发布结果。

组织名有大写字母时，网站仓库名仍必须使用小写 roboneuxs.github.io。此新仓库采用从 main 根目录发布，不需要额外创建 clock.yml。
该包包含新版布局、VS Code 风格高亮、格式整理后的源码、MQTT 控制和名称保存。网页可以直接从 index.html 运行；MQTT 连接需要网络。
本地打包和 ZIP 校验已完成，不代表文件已经上传或网页已经上线。

GitHub 官方说明：
https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
