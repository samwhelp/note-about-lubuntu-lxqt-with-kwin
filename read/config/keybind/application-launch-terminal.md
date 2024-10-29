---
title: 開啟應用程式 (Terminal)
nav_order: 5010
has_children: false
parent: 按鍵綁定
grand_parent: 設定
---


# 開啟應用程式 (Terminal)

> [lubuntu-lxqt-with-kwin 微調腳本](https://github.com/samwhelp/lubuntu-lxqt-with-kwin-adjustment/tree/main/prototype/main/lxqt-config/Main)




## 主題

* [一般終端機](#一般終端機)
* [相關議題](#相關議題)




## 一般終端機

| 按鍵組合          | 功能         | 執行指令                     |
| ----------------- | ------------- | --------------------------- |
| `Alt + Enter`     | 開啟 Terminal | `sakura`                    |


| 按鍵組合          | 功能         | 執行指令                     |
| ----------------- | ------------- | --------------------------- |
| `Alt + Shift + a` | 開啟 Terminal | `sakura`                    |
| `Alt + Ctrl + a`  | 開啟 Terminal | `xfce4-terminal`            |


| 按鍵組合          | 功能         | 執行指令                     |
| ----------------- | ------------- | --------------------------- |
| `Alt + Shift + t` | 開啟 Terminal | `konsole`                   |
| `Alt + Ctrl + t`  | 開啟 Terminal | `qterminal`                 |


* [設定片段: ~/.config/lxqt/globalshortcutsrc](https://github.com/samwhelp/lubuntu-lxqt-with-kwin-adjustment/blob/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/lxqt/globalkeyshortcuts.conf#L265-L288)

``` ini
[Alt%2BShift%2BT]
Comment=Terminal
Enabled=false
Exec=konsole

[Alt%2BControl%2BT]
Comment=Terminal
Enabled=true
Exec=qterminal

[Alt%2BReturn]
Comment=Terminal
Enabled=true
Exec=sakura

[Alt%2BShift%2BA]
Comment=Terminal
Enabled=true
Exec=sakura

[Alt%2BControl%2BA]
Comment=Terminal
Enabled=true
Exec=xfce4-terminal
```




## 相關議題

* [鍵盤按鍵綁定 / 開啟常用的應用程式](https://samwhelp.github.io/note-about-lubuntu-lxqt-with-kwin/read/config/keybind/application-launch-favorite.html)
