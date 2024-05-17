<p align="center">
  <img alt="Fluid Logo" src="https://avatars2.githubusercontent.com/t/3419353?s=280&v=4" width="128">
</p>
<p align="center">谷月修改版的 Fluid 主题</p>
<p align="center">Fluid theme edited by Kukmoon</p>

![预览](https://img.kukmoon.com/202111262037388.png)



<p align="center"> <a title="原版主题" href="https://github.com/fluid-dev/hexo-theme-fluid">点击这里跳转到原版主题</a></p>

## 修改内容

1. 增加了打赏模块，详见[这里](https://blog.kukmoon.com/7bf76e1d.html)。
2. 增加了“分享到”模块，详见[这里](https://blog.kukmoon.com/c87ddd18.html)。
3. 在 GitHub 上 Fork 了[原版的 Fluid 主题](https://github.com/fluid-dev/hexo-theme-fluid)，用 Git 和 GitHub 进行版本控制。
4. 修改了 `Readme.md`，以后每次更新都会修改 `Readme.md`。
5. ~~在首页增加了一个列表，列出主站和镜像站的 URLs，详见[这里](https://blog.kukmoon.com/45ee46db.html)。~~
6. ~~在每篇文章的开头增加了一个提示，提示用户可以点击跳转到镜像站，详见[这里](https://blog.kukmoon.com/c4d07859.html)。~~
7. 修改了“分享到”模块，详见[这里](https://blog.kukmoon.com/c87ddd18.html)。
8. 代码高亮设置为 Mac 风格。
9. 升级到 hexo-theme-fluid 1.9.6，并且增加了打赏、“分享到”模块。将打赏模块另存为 `themes/fluid/layout/_partials/donate.ejs`，将“分享到”模块另存为 `themes/fluid/layout/_partials/share.ejs`，并将它调用的 `jquery.min.js`、`qrcode.min.js`、`social-share.min.js` 复制到 `themes/fluid/source/js` 目录，将它调用的 `social-share.min.css` 复制到 `themes/fluid/source/css` 目录，并在 `_config.fluid.yml` 文件中引入这个 CSS 文件，最后在 `themes/fluid/layout/post.ejs` 文件中加入以下代码：
    ```
    <div>
        <!-- 引入自己编写的“分享到”模块（新） -->
        <%- partial('_partials/share') %>            
        <hr/>
        <!-- 引入自己编写的打赏模块（新） -->
        <%- partial('_partials/donate') %>
        <hr/>
    </div>
    ```
10. 参照[这篇文章](http://lzqlearn.com/blog/6560820db005/)，设计了 Mac 风格代码块，把 CSS 代码写在了 `theme/fluid/css/macpanel-highlightjs.css` 文件中，并在 `_config.fluid.yml` 文件中引入这个 CSS 文件。

## 涉及的文件

新增的文件：

```
layout/_partials/donate.ejs
layout/_partials/share.ejs
source/css/macpanel-highlightjs.css
source/css/macpanel-prismjs.css
source/css/social-share.min.css
source/js/jquery.min.js
source/js/qrcode.min.js
source/js/social-share.min.js
```

修改的文件：

```
layout/post.ejs
README.md
README_en.md
```

把它们打包到 `fluid_modified_files.zip` 当中。

## 鸣谢

+ [感谢 Notepad++ 提供开发工具](https://github.com/notepad-plus-plus/notepad-plus-plus)
+ [感谢 Social-share.js 提供“分享到”模块](https://github.com/slince/social-share.js)
+ [感谢 廖雪峰老师的 Git 教程](https://www.liaoxuefeng.com/wiki/896043488029600)
+ [感谢 微软公司 提供开发工具 VSCode]()


## To Do

1. 给首页增加一个响应式的侧边栏，点击按钮才出现，否则隐藏。
2. 给首页每篇文章之间增加分割线，增加它们之间的距离。
