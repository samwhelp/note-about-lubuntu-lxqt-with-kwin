---
title: 開啟應用程式 (常用的)
nav_order: 5013
has_children: false
parent: 按鍵綁定
grand_parent: 設定
---


# 開啟應用程式 (常用的)

> [lubuntu-lxqt-with-kwin 微調腳本](https://github.com/samwhelp/lubuntu-lxqt-with-kwin-adjustment/tree/main/prototype/main/lxqt-config/Main)




## 主題

* [常用的應用程式](#常用的應用程式)
* [其他](#其他)
* [相關議題](#相關議題)



## 常用的應用程式

| 按鍵組合           | 功能            | 執行指令                         |
| ------------------ | --------------- | -------------------------------- |
| `Alt + Shift + f`  | 開啟檔案管理器  | `pcmanfm-qt`             |
| `Alt + Shift + g`  | 開啟檔案管理器  | `thunar`                     |
| `Alt + Shift + e`  | 開啟文字編輯器  | `featherpad`              |
| `Alt + Shift + b`  | 開啟網頁瀏覽器  | `firefox --new-tab about:blank`  |
| `Alt + Shift + s`  | 開啟系統設定    | `lxqt-config`                |


* [設定片段: ~/.config/lxqt/globalshortcutsrc](https://github.com/samwhelp/lubuntu-lxqt-with-kwin-adjustment/blob/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/lxqt/globalkeyshortcuts.conf#L290-L308)

``` ini
[Alt%2BShift%2BF]
Comment=File Manager
Enabled=true
Exec=pcmanfm-qt

[Alt%2BShift%2BG]
Comment=File Manager
Enabled=true
Exec=thunar

[Alt%2BShift%2BE]
Comment=Text Editor
Enabled=true
Exec=featherpad

[Alt%2BShift%2BB]
Comment=Web Browser
Enabled=true
Exec=firefox, --new-tab, about:blank
```


``` ini
[Alt%2BShift%2BS]
Comment=System Settings
Enabled=true
Exec=lxqt-config
```




## 其他

> 可以按下「`Alt + F1`」執行「`lubuntu-lxqt-with-kwin-launcher`」，就可以找到其他的「應用程式」來執行




## 相關議題

* [鍵盤按鍵綁定 / 開啟終端機](https://samwhelp.github.io/note-about-lubuntu-lxqt-with-kwin/read/config/keybind/application-launch-terminal.html)
