[[How Obsidian Stores Data]]
# Obsidian如何存储数据

我们相信 [[Obsidian简介#我们的优势|您的数据始终由您拥有和控制]]。
您的笔记以markdown格式存储，markdown是基于纯文本的开放的文件格式，因此，将来任何能够处理文本文档的计算机都应该可以读取。
您甚至可以在Obsidian中打开笔记，同时在其他软件中自由的编辑笔记。

但是，仍然会有一些软件所需的数据无法存储于markdown文档中。Obsidian 会在您的库目录中创建一个名为 `.obsidian` 文件夹。其中包含您的配置数据，有自定义热键、启用插件记录等信息。在大多数系统上，任何以`.` 开头的目录都是不可见的，因此，除非专门设置显示隐藏的文件夹，否则您将永远看不到它。如果删除此目录，虽然不会丢失所有数据，但您将丢失那些自定义设置。再次在Obsidian中打开该库目录时，将重新创建该数据文件夹。如果您使用的是`git`, 最好 `忽略` 这个 `.obsidian` 文件夹，因为缓存更新速度足够快，会使提交变得困难，目前我们还未观察到所引发的其它问题。

如果使用自定义CSS， Obsidian 将在库目录中创建一个 `obsidian.css` 。更多有关信息， 请参见[[自定义CSS]]。

Obsidian 还将一些信息存储在系统目录中。每个操作系统都不同：
在Mac系统中，它是 `/Users/yourusername/Library/Application Support/obsidian`；
在Windows系统中是 `%APPDATA%\Obsidian\`；
在Linux系统中是 `$XDG_CONFIG_HOME/Obsidian/` 或 `~/.config/Obsidian/` 。
因此，建议不要在以上目录中创建文件夹或存放数据。

除此以外，您可以在操作系统允许的任何位置创建库目录。Obsidian 文件可以用 Dropbox， iCloud， OneDrive， git 以及我们迄今为止尝试过的所有其他同步服务（国内推荐坚果云）很好的同步。

