这个项目是使用[Hexo](https://hexo.io/)来搭建自己的[博客](https://willmajor.github.io/)，并通过[Github Pages](https://pages.github.com/)来实现部署和访问。

- 分支master：包含项目源代码
- 分支gh-pages：包含使用hexo生成的静态网站代码

常用命令

#### 创建新博客

``` bash
$ hexo new "My New Post"
```

More info: [Writing](https://hexo.io/docs/writing.html)

#### 本地预览（端口4000）

``` bash
$ hexo server | hexo s
```

More info: [Server](https://hexo.io/docs/server.html)

#### 生成静态资源文件

``` bash
$ hexo generate | hexo g
```

More info: [Generating](https://hexo.io/docs/generating.html)

#### 部署静态资源文件
根据`_config.yaml`文件中的`deployment`配置，推送代码到远程分支`gh-pages`

``` bash
$ hexo deploy | hexo d
```

More info: [Deployment](https://hexo.io/docs/one-command-deployment.html)
