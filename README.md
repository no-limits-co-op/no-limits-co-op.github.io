### 博客安装及运行

博客通过 [jekyll](https://jekyllrb.com/) 搭建，所以需要 ruby 环境。准备好 ruby 环境后，安装相关的 gem 依赖。

```shell
bundle install
```
依赖安装完成后，可以在本地运行下列命令运行 jekyll，然后访问 *http://localhost:4000/* 预览编译后的静态页面。

```shell
bundle run jekyll serve
```
### 配置

此博客使用了 jekyll 的 [minimal-mistakes](https://github.com/mmistakes/minimal-mistakes) 主题。该主题扩展性比较高，搭建也比较简单，如果需要修改相关配置可以参考该主题的[配置说明](https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/)。

#### 目前使用的配置

- [关于我们] 导航栏。在 *_data/navigation.yml* 文件中配置，这个文件负责配置博客导航栏的内容，相关配置项可以查看[导航栏配置](https://mmistakes.github.io/minimal-mistakes/docs/navigation/)。
- 搜索功能。目前搜索功能使用的是默认议案 [lunr](https://lunrjs.com/)，博客中只要在 *_config.yml* 中开启配置即可，具体配置项可查看[搜索功能配置](https://mmistakes.github.io/minimal-mistakes/docs/configuration/#site-search)。
- 文章页面默认布局配置。在 *_config.yml* 中配置了 `defaults` 项，分别配置了 *_posts* 和 *_pages* 的默认布局。具体可查看 [posts 配置](https://mmistakes.github.io/minimal-mistakes/docs/posts/)和 [pages 配置](https://mmistakes.github.io/minimal-mistakes/docs/pages/)。
- 文章作者配置。作者信息可以统一编写在 *_data/authors.yml* 文件中，然后在自己编写的文章声明信息中配置 `author: author_name` 即可。

