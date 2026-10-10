# 手动发布到现有 GitHub Pages

目标仓库：https://github.com/dreamcather726/esp32s3-pages-test
网页地址：https://dreamcather726.github.io/esp32s3-pages-test/clock.html

1. 解压 github-pages-publish.zip。进入仓库 main 分支，点击 Add file → Upload files，将 index.html、clock.html、sensor-experiments.zip 三个文件拖入页面，点击 Commit changes 提交到 main。
2. 打开仓库原有的 .github/workflows/clock.yml，点击铅笔编辑。用解压文件夹里的 clock.yml 全部内容替换原内容，再点击 Commit changes 提交到 main。注意它仍放在 .github/workflows/clock.yml，不能上传到根目录。
3. 打开仓库 Actions，等待 Publish sensor experiments 变绿，再访问原网页地址。若看到旧版，用 Ctrl+F5 刷新。

必须替换旧 workflow：旧时钟流程会尝试提取和编译时钟固件，而新版是可独立运行的实验现象演示页。
clock.html 和 index.html 内容相同，无外部运行依赖。sensor-experiments.zip 包含完整传感器示例代码及接线文件。
本包已在本地准备并校验，不代表已经发布成功。不要改动仓库其他文件或 Pages 发布设置。
