---
title: 系統選單
nav_order: 5002
has_children: false
parent: 按鍵綁定
grand_parent: 設定
---


# 系統選單

> [lubuntu-lxqt-with-kwin 微調腳本](https://github.com/samwhelp/lubuntu-lxqt-with-kwin-adjustment/tree/main/prototype/main/lxqt-config/Main)




## 主題

* [顯示「應用程式啟動選單」](#顯示應用程式啟動選單)
* [顯示「視窗操作選單」](#顯示視窗操作選單)
* [顯示「所有開啟視窗預覽」](#顯示所有開啟視窗預覽)




## 顯示「應用程式啟動選單」

| 按鍵組合          | 功能                     | 執行指令                           |
| ----------------- | ------------------------ | ---------------------------------- |
| `Alt + F1`        | 顯示「應用程式啟動選單」 | `path=/panel/fancymenu/show_hide`  |


> 因為我個人會使用「`Win鍵`」搭配「其他鍵」當作「組合鍵」來做一些操作，為了避免干擾，

> 所以使用「Win鍵」顯示「開始功能表」的功能被我停用了。

> 請參考『[停用「Win鍵」開啟「開始功能表」](https://samwhelp.github.io/note-about-kubuntu/read/howto/disable-opening-application-launcher-with-super-key.html)』


* [設定片段: ~/config/lxqt/globalkeyshortcuts.conf](https://github.com/samwhelp/lubuntu-lxqt-with-kwin-adjustment/blob/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/lxqt/globalkeyshortcuts.conf#L11-L13)

``` ini
[Alt%2BF1]
Comment=Show/hide main menu
Enabled=true
path=/panel/fancymenu/show_hide

```




## 顯示「視窗操作選單」

* [設定片段](https://github.com/samwhelp/lubuntu-lxqt-with-kwin-adjustment/blob/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/kglobalshortcutsrc#L144)

| 按鍵組合           | 功能                 | 執行指令                  |
| ------------------ | -------------------- | ------------------------- |
| `Alt + F3`         | 顯示「視窗操作選單」 | `Window Operations Menu=` |
| `Alt + Space`      | 顯示「視窗操作選單」 | `Window Operations Menu=` |


> 也可以在「視窗標題列」使用「滑鼠右鍵」，就會顯示「視窗操作選單」。


* [設定片段: ~/.config/kglobalshortcutsrc](https://github.com/samwhelp/lubuntu-lxqt-with-kwin-adjustment/blob/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/kglobalshortcutsrc#L138)

``` sh
Window Operations Menu=Alt+Space\tAlt+F3,Alt+F3,Window Operations Menu
```




## 顯示「所有開啟視窗預覽」

| 按鍵組合          | 功能                     | 執行指令             |
| ----------------- | ------------------------ | -------------------- |
| `Win + c`         | 顯示「所有開啟視窗預覽」 | `ExposeAll=`         |


* [設定片段: ~/.config/kglobalshortcutsrc](https://github.com/samwhelp/lubuntu-lxqt-with-kwin-adjustment/blob/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/kglobalshortcutsrc#L49)

``` sh
ExposeAll=Ctrl+F10\tMeta+C\tLaunch (C),Ctrl+F10\tLaunch (C),Toggle Present Windows (All desktops)
```




## lxqt-runner

| 按鍵組合          | 功能              | 執行指令                         |
| ----------------- | ----------------- | -------------------------------- |
| `Alt + F2`        | 執行 lxqt-runner  | `path=/runner/show_hide_dialog`  |

* [設定片段: ~/config/lxqt/globalkeyshortcuts.conf](https://github.com/samwhelp/lubuntu-lxqt-with-kwin-adjustment/blob/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/lxqt/globalkeyshortcuts.conf#L15-L18)

``` ini
[Alt%2BF2]
Comment=Show/hide runner
Enabled=true
path=/runner/show_hide_dialog
```
