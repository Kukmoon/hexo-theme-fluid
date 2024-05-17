<p align="center">
  <img alt="Fluid Logo" src="https://avatars2.githubusercontent.com/t/3419353?s=280&v=4" width="128">
</p>
<p align="center">Fluid theme edited by Kukmoon</p>

![Preview](https://img.kukmoon.com/202111262037388.png)




<p align="center"> <a title="Original Theme" href="https://github.com/fluid-dev/hexo-theme-fluid">Click here to visit the original theme</a></p>

## Version

**1.9.4**

## What are Modified?

1. A donation module was added. See [here](https://blog.kukmoon.com/7bf76e1d.html) for details.
2. A "Share to" module was added. See [here](https://blog.kukmoon.com/c87ddd18.html).
3. [The original Fluid theme](https://github.com/fluid-dev/hexo-theme-fluid) was forked at GitHub to use Git and GitHub for version control.
4. `Readme.md` was updated. Every update will modify `Readme.md` in future.
5. <del>Added a list of URLs for the main and mirror sites on the front page, see [here](https://blog.kukmoon.com/45ee46db.html) for details.</del>
6. <del>Added a prompt at the beginning of each article to indicate that users can click to jump to the mirror site, see [here](https://blog.kukmoon.com/c4d07859.html) for more details.</del>
7. The "Share to" module was modified. See [here](https://blog.kukmoon.com/c87ddd18.html).
8. The code highlighting is set to Mac style.
9. Upgraded to hexo-theme-fluid 1.9.6. The donation and "Share to" modules were once again added. The donation module was saved as `themes/fluid/layout/_partials/donate.ejs`. The "Share to" module was saved as `themes/fluid/layout/_partials/share.ejs`. The dependencies, including `jquery.min.js`, `qrcode.min.js` and `social-share.min.js` were copied to `themes/fluid/source/js` folder. Another dependency, `social-share.min.css` that was copied to `themes/fluid/source/css` folder, was quoted within `_config.fluid.yml`. Finally, the following codes were added into `themes/fluid/layout/post.ejs` :
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
10. New code block was redesigned as an Mac style according to [this article](http://lzqlearn.com/blog/6560820db005/). CSS codes is stored in `theme/fluid/css/macpanel-highlightjs.css`. The style sheet is quoted within `_config.fluid.yml`.

## Files involved

Added files:

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

Modified files：

```
layout/post.ejs
README.md
README_en.md
```

All files above is compacted into `fluid_modified_files.zip`.

## Acknowledgements

+ <del>[Thanks to Notepad++ for providing development tool](https://github.com/notepad-plus-plus/notepad-plus-plus)</del>
+ [Thanks to Social-share.js for providing the "Share to" module](https://github.com/slince/social-share.js)
+ [Thanks to Xuefeng Liao for the Git tutorial](https://www.liaoxuefeng.com/wiki/896043488029600)
+ [Thanks to Microsoft for providing development tool, VSCode](https://code.visualstudio.com/)

## To Do

1. To add a responsive sidebar to the home page, which appears only when the button is clicked, otherwise it is hidden.
2. To add a split line between each article on the homepage and also increase the distance between them.

Translated with www.DeepL.com/Translator (free version)