## 如何使用 Planet BKT

为了方便，Planet BKT 使用了 [HUGO](https://gohugo.io/) 作为文章平台工具，进行文章的静态生成，并最终利用 GitHub Pages 呈现网页，故整个过程你只需按照 HUGO 的正常使用方式进行使用即可。大致常用命令如下（在此源码仓库的根目录下执行）：

```
$ hugo server # 启动一个本地服务器，预览目前状态下的网站内容
$ hugo new posts/my-post.md # 创建一篇新文章，以便进行编辑
$ hugo server -D # 启用本地服务器，并且能够预览状态为草稿（`draft: true`）的文章
$ hugo -D # 生成静态页面（如果需要），生成的文件将位于 public 目录下
```

创建文章时，创建格式为 `<分类>/<文件名>.<格式>`，上面给出的例子中，分类为 posts，文件名为 my-post，格式为 md （markdown）。创建文章后，默认会使用 [YAML front-matter](https://gohugo.io/content-management/front-matter/) 标记文章的一些元信息，请留意 draft 草稿状态的文章最终不会显示。

若要获取 HUGO，请参考[官方文档给出的安装方式](https://gohugo.io/getting-started/installing)。

## 文章内容指导建议

Planet BKT 可供所有 BKT 成员分享其文章，下面为文章内容方面相关的指导意见。

您可以自由选择您的文章是否发布到 Planet BKT，对于发布到 Planet BKT 的文章，您也可以自由的选择文章所使用的共享许可，此处不做任何限制。

您所分享到 Planet BKT 的文章需要与 BKT 具有一定程度的相关性。您可以通过“BKT 中除自己之外是否有其他至少一人对此文章的主题感兴趣”来做出判断。

在发布您的文章时，建议使用标签来标记您文章所相关的主题，以便读者更方便的查阅您的文章。例如 `tags: ["ballance"]` 或 `tags: ["自由软件", "音乐制作"]`。

## 改善 Planet BKT

Planet BKT 作为一个实验性的文章聚合平台，目前其实和 Planet KDE 之类的形式上是有差异的。Planet BKT 需要主动的创建文章并提交到仓库中来完成发布，而不象是 RSS 聚合平台样可以通过直接提供 RSS 来使得此平台自动获取文章并呈现文章的聚合。若你对此方面的功能感兴趣并希望尝试实现，可以直接进行改善。

Planet BKT 使用了 [geekblog](https://themes.gohugo.io/hugo-geekblog/) 主题（基于 `v0.5.3`，有改动），但并不一定完整的符合我们的需求，若你有任何建议，可以进行讨论并修改或提供更适合的主题。
