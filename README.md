# nexinmap-downloader-ci

这个仓库只负责编译安装包，不存放产品源代码。

在 Actions 里手动运行 **Build installers**。流水线会从私有 Gitee 仓库拉取源码，在 GitHub 的 Windows、Linux、macOS 机器上编译，再把安装包上传到公开仓库 [nexin-map-download-releases](https://gitee.com/liu-bofang/nexin-map-download-releases)。

需要在本仓库的 Actions Secrets 中配置 `GITEE_TOKEN`。该令牌要能读取私有源码仓库，并能向发布仓库创建 Release、上传附件。
