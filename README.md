# nexinmap-downloader-ci

公开仓库，只负责编译并发布安装包。产品源码在私有仓库 [nexinmap-downloader](https://github.com/ShareQiu1994/nexinmap-downloader)。

在 Actions 里手动运行 **Build installers**。流水线用 Secret `SOURCE_TOKEN` 读取私有源码，在 GitHub 的 Windows、Linux、macOS 上编译，再把安装包挂到本仓库的 Releases。

检查更新先读镜像 `https://nexinmap.com/packages/latest/update.json`，打不开再读 GitHub Release。
