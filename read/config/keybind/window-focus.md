---
title: 視窗聚焦切換
nav_order: 5025
has_children: false
parent: 按鍵綁定
grand_parent: 設定
---


# 視窗聚焦切換

> [lubuntu-lxqt-with-kwin 微調腳本](https://github.com/samwhelp/lubuntu-lxqt-with-kwin-adjustment/tree/main/prototype/main/lxqt-config/Main)




## 主題

* [前後聚焦切換](#前後聚焦切換)
* [前後聚焦切換 (Alternative)](#前後聚焦切換-alternative)




## 前後聚焦切換

| 按鍵組合    | 功能                    | 執行指令                           |
| ----------- | ----------------------- | ---------------------------------- |
| `Win + a`   | 聚焦切換到前面一個視窗  | `Walk Through Windows (Reverse)=`  |
| `Win + s`   | 聚焦切換到後面一個視窗  | `Walk Through Windows=`            |


> 關於「`Win + s`」就是知名「`Alt + Tab`」的功能。


* [設定片段: ~/.config/kglobalshortcutsrc](https://github.com/samwhelp/lubuntu-lxqt-with-kwin-adjustment/blob/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/kglobalshortcutsrc#L111-L112)

``` sh
Walk Through Windows=Meta+S,Alt+Tab,Walk Through Windows
Walk Through Windows (Reverse)=Meta+A,Alt+Shift+Backtab,Walk Through Windows (Reverse)
```


> 目前這組切換的顯示效果，是設定採用「`big_icons`」。


> 關於「`big_icons`」是放在「`/usr/share/kwin/tabbox/big_icons`」這個資料夾。


* [設定片段: ~/.config/kwinrc](https://github.com/samwhelp/lubuntu-lxqt-with-kwin-adjustment/blob/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/kwinrc#L55-L56)

``` ini
[TabBox]
LayoutName=big_icons
```




## 前後聚焦切換 (Alternative)

| 按鍵組合     | 功能                    | 執行指令                                       |
| ------------ | ----------------------- | ---------------------------------------------- |
| `Win + Esc`  | 聚焦切換到前面一個視窗  | `Walk Through Windows Alternative=`            |
| `Alt + Esc`  | 聚焦切換到後面一個視窗  | `Walk Through Windows Alternative (Reverse)=`  |


* [設定片段: ~/.config/kglobalshortcutsrc](https://github.com/samwhelp/lubuntu-lxqt-with-kwin-adjustment/blob/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/kglobalshortcutsrc#L113-L114)

``` sh
Walk Through Windows Alternative=Meta+Esc,none,Walk Through Windows Alternative
Walk Through Windows Alternative (Reverse)=Alt+Esc,none,Walk Through Windows Alternative (Reverse)
```


> 目前這組切換的顯示效果，是設定採用「`coverswitch`」。


> 關於「`coverswitch`」是放在「`/usr/share/kwin/tabbox/coverswitch`」這個資料夾。


* [設定片段: ~/.config/kwinrc](https://github.com/samwhelp/lubuntu-lxqt-with-kwin-adjustment/blob/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/kwinrc#L58-L59)

``` ini
[TabBoxAlternative]
LayoutName=coverswitch
```




## 用法對照

* [工作空間切換](https://samwhelp.github.io/note-about-lubuntu-lxqt-with-kwin/read/config/keybind/workspace-switch.html)
