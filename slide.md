
# [Sublime Text 2][site]

[site]: http://www.sublimetext.com/

---

# Landslide

[Github](https://github.com/adamzap/landslide)

Generate HTML5 slideshows from markdown, ReST, or textile.

Landslide is primarily written in Python, but it's themes use:

* HTML5
* Javascript
* CSS

# Installation
    
    !bash
    pip install landslide
    landslide this.md

---

# Blogs

[Sublime Text 2 入门及技巧](http://lucifr.com/139225/sublime-text-2-tricks-and-tips/)

[Sublime Text 2 - 性感无比的代码编辑器](http://www.iplaysoft.com/sublimetext.html)

[Sublime Text 2 - 好用的跨平台代码编辑器 Part.1 介绍](http://motype.org/2012/07/sublime-text-2-intro/)

---

# Installation

[Buy...](http://www.sublimetext.com/buy)

[Download][download]
    
    !bash
    wget http://c758482.r82.cf2.rackcdn.com/Sublime%20Text%202.0.1%20x64.tar.bz2

[PPA “WebUpd8” team - Sublime Text 2][ppa]
    
    !bash
    sudo add-apt-repository ppa:webupd8team/sublime-text-2 
    sudo apt-get update
    sudo apt-get install sublime-text-dev

[download]: http://www.sublimetext.com/download
[ppa]: https://launchpad.net/~webupd8team/+archive/sublime-text-2

---

# UI

## Python Console

    ctrl backquote

    view.settings().get('font_face')
    sublime.packages_path()

## Command Palette
  
    shift + command + p

## Goto Anything

    command + p
    # 文件的内容
    @ active buffer
    : 指定行数

---

# [Reference][reference]

[reference]: https://sublime-text-unofficial-documentation.readthedocs.org/en/latest/reference/reference.html

---

# Settings

Preferences -> Settings - Default

Preferences -> Settings - User
    
    !json
    {
      "font_face": "wenquanyi micro hei mono",
      "font_size": 10,
      "ignored_packages":
      [
        "Vintage",
        "BracketHighlighter"
      ],
      "indent_guide_options":
      [
        "draw_active"
      ],
      "tab_size": 2,
      "translate_tabs_to_spaces": true
    }

---

# [Sublime Package Control](http://wbond.net/sublime_packages/package_control)

* [SublimeREPL](https://github.com/wuub/SublimeREPL)
* [sublime-text-2-git](https://github.com/kemayo/sublime-text-2-git/wiki)
* [Vintage Mode](http://www.sublimetext.com/docs/2/vintage.html)
* [BracketHighlighter](https://github.com/facelessuser/BracketHighlighter)

---

# Develop

    ~/.config/sublime-text-2

[Sublime Info - Information about Sublime Text 2][info]

[Sublime Text Unofficial Documentation][unofficial]

[Sublime Text 2 Documentation][doc]

[Perfect Workflow in Sublime Text 2][video]

[doc]: http://www.sublimetext.com/docs/2/
[info]: http://www.sublimetext.info/
[unofficial]: http://docs.sublimetext.info/en/latest/index.html
[video]: https://tutsplus.com/course/improve-workflow-in-sublime-text-2/

---

# Shorcuts

Preferences -> Key Bindings - Default

Preferences -> Key Bindings - User

    !json
    {
      "keys": ["["],
      "command": "insert_snippet",
      "args": {
        "contents": "[$0]"
      },
      "context": [{
        "key": "setting.auto_match_enabled",
        "operator": "equal",
        "operand": true
      }, {
        "key": "selection_empty",
        "operator": "equal",
        "operand": true,
        "match_all": true
      }, {
        "key": "following_text",
        "operator": "regex_contains",
        "operand": "^(?:\t| |\\)|]|;|\\}|$)",
        "match_all": true
      }]
    }

---

# 实用快捷键

[Sublime Text 2 实用快捷键][mac]

[Keyboard Shortcuts - Windows/Linux][linux]

[mac]: http://lucifr.com/139235/sublime-text-2-useful-shortcuts/
[linux]: http://docs.sublimetext.info/en/latest/reference/keyboard_shortcuts_win.html

---

# Search
  
## ctrl d
* ctrl u
* ctrl k

## ctrl f
* f2
* shift f2
* alt f2

## ctrl shift f 
* f4
* shift f4

---

# Other

* ctrl alt q 录制和结束录制宏
* ctrl alt shift q 播放宏

## 多个光标

* alt shift up
* ctrl mouse
