Sublime Text 3 安装配置
====

Sublime Text 大概是最流行的文本/代码编辑器。目前的稳定版是 2.0.2，3 目前仍是 beta(build 3083)，不过已经完全可以替代 2 来用了。

下载安装
----

Sublime Text 3 提供了 OSX、Windows(32/64)、Linux(32/64) 多个桌面平台的安装包，下载后安装或解压缩即可。

配置
----

### 1. 用户配置

Sublime Text 的配置是基于 JSON 的配置文件，并没有提供 GUI 面板，所以我们需要通过编辑这份配置文件来配置它。

打开菜单 Preferences-->Settings--Default，可以看到一份几百行的 JSON 文件，这就是 Sublime Text 支持的所有配置选项。所有的配置选项都有详细的说明，而且选项命名比较规范，容易看懂。

上面这份文件是 Sublime Text 的默认配置，用户不能修改它。如果要修改配置，需要打开菜单 Preferences-->Settings--User，在这份用户配置中添加、删除或修改配置选项。

一些常规的配置：

```json
"font_face": "Monaco",            // 编辑器的字体
"font_size": 14,                  // 字号
"highlignt_line": true,           // 是否高亮当前行
"tab_size": 2,                    // tab 字符宽度（对应的空格数）
"translate_tabs_to_spaces": true, // 是否自动将新插入的 tab 转换为空格
"word_wrap": true                 // 是否自动换行
```

### 2. 包管理器

包管理器被广泛应用在系统（Linux 中的 apt/yum）、工具（Atom 中的 apm）和编程语言（Node.js 中的 npm）中，Sublime Text 的包管理器是 [Sublime Package Control](https://packagecontrol.io/)，它由第三方提供。

Package Control 可以用来安装/卸载插件、主题，并保持插件、主题的自动更新。你也可以编写自己的插件或主题，并[发布](https://packagecontrol.io/docs/submitting_a_package)到 Package Control 上。

参考 [Installation](https://packagecontrol.io/installation) 来安装 Package Control。

#### 安装插件

在 Sublime Text 中执行快捷键 `Ctrl+Shift+P`，打开命令栏。输入 "install package"，通过键盘 `↑` `↓` 键将光标定位到 'Package Control: Install Package' 选项，点击回车；或者直接用鼠标点击该选项。

短暂的加载后，会展示出可用的插件、主题列表。输入要安装的包名（这里用 'emmet' 来演示，将光标定位到指定的选项，点击回车即可开始安装。Sublime Text 底部状态栏的左下角会显示安装进度。

#### 卸载插件

执行快捷键 `Ctrl+Shift+P`，打开命令栏。输入 'remove package'，执行 'Package Control: Remove Package' 选项，这里会列出所有已安装的包。将光标定位到要删除的选项，点击回车即可执行卸载。

### 3. 推荐一些插件和主题

插件：

+ [Emmet](https://github.com/sergeche/emmet-sublime) Emmet 的 Sublime 支持
+ [HTML-CSS-JS Prettify](https://github.com/victorporof/Sublime-HTMLPrettify) 可以用来格式化 HTML/CSS/JS 代码
+ [LESS](https://github.com/danro/Less-sublime) 提供了 LESS 代码的高亮

主题：

+ [Theme - Soda](https://github.com/buymeasoda/soda-theme/) 提供了黑、白两种颜色的主题，比较细腻
+ [Material Theme](https://github.com/equinusocio/material-theme) 遵循 Material Design 的主题，提供了三种配色
