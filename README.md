# kiz-lang-website
The website of the kiz programming language

**website**: [kiz.i2pl.com](http://kiz.i2pl.com)

下载页通过 GitHub API 动态解析 [kizi releases](https://github.com/kiz-lang/kizi/releases/latest) 的最新三平台资产(Windows/Linux/macOS),发布新版本后页面自动跟随,无需手动改链接。

## 文档站

[docs.html](https://kiz.i2pl.com/docs.html) 渲染 kizi 主仓库 `docs/` 的 markdown 文档。为保证大陆网络可访问,文档内容是**本仓库 `docs/` 目录的副本**(同域拉取,不依赖 GitHub API/raw)。

同步方式:在 Actions 页手动运行 **Sync docs from kizi** 工作流,它会从 kizi 主仓库拉取最新文档并自动提交。新增文档时需在 `docs.html` 的 `DOC_ORDER` 列表中登记。
