---
title: 系統操作
nav_order: 5001
has_children: false
parent: 按鍵綁定
grand_parent: 設定
---


# 系統操作

> [lubuntu-lxqt-with-kwin 微調腳本](https://github.com/samwhelp/lubuntu-lxqt-with-kwin-adjustment/tree/main/prototype/main/lxqt-config/Main)




## 主題

* [切換「顯示桌面」](#切換顯示桌面)
* [離開系統選單](#離開系統選單)
* [登出確認對話框](#登出確認對話框)
* [鎖住螢幕](#鎖住螢幕)
* [顯示「工作空間選單」](#顯示工作空間選單)
* [切換「顯示目前工作空間的所有視窗預覽」](#切換顯示目前工作空間的所有視窗預覽)




## 切換「顯示桌面」

| 按鍵組合           | 功能             | 執行指令             |
| ------------------ | ---------------- | -------------------- |
| `Win + d`          | 切換「顯示桌面」 | `Show Desktop=`      |


* [設定片段: ~/.config/kglobalshortcutsrc](https://github.com/samwhelp/lubuntu-lxqt-with-kwin-adjustment/blob/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/kglobalshortcutsrc#L62)

``` sh
Show Desktop=Meta+D,Meta+D,Show Desktop
```




## 離開系統選單

| 按鍵組合           | 功能                 | 執行指令               |
| ------------------ | -------------------- | ---------------------- |
| `Alt + Shift + z`  | 顯示「離開系統選單」 | `lxqt-leave`  |


* [設定片段: ~/.config/lxqt/globalkeyshortcuts.conf](https://github.com/samwhelp/lubuntu-lxqt-with-kwin-adjustment/blob/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/lxqt/globalkeyshortcuts.conf#L240-L243)

``` ini
[Alt%2BShift%2BZ]
Comment=Leave
Enabled=true
Exec=lxqt-leave
```




## 登出確認對話框

| 按鍵組合           | 功能                 | 執行指令               |
| ------------------ | -------------------- | ---------------------- |
| `Alt + Shift + x`  | 顯示「登出確認對話框」 | `lxqt-leave --logout`  |


* [設定片段: ~/.config/lxqt/globalkeyshortcuts.conf](https://github.com/samwhelp/lubuntu-lxqt-with-kwin-adjustment/blob/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/lxqt/globalkeyshortcuts.conf#L245-L248)

``` ini
[Alt%2BShift%2BX]
Comment=Logout
Enabled=true
Exec=lxqt-leave, --logout
```




## 鎖住螢幕

| 按鍵組合           | 功能         | 執行指令              |
| ------------------ | ------------ | --------------------- |
| `Alt + Shift + l`  | 鎖住螢幕     | `lxqt-leave --lockscreen` |


* [設定片段: ~/.config/lxqt/globalshortcutsrc](https://github.com/samwhelp/lubuntu-lxqt-with-kwin-adjustment/blob/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/lxqt/globalkeyshortcuts.conf#L235-L238)

``` ini
[Alt%2BShift%2BL]
Comment=Lock screen
Enabled=true
Exec=lxqt-leave, --lockscreen
```



## 顯示「工作空間選單」

| 按鍵組合          | 功能                 | 執行指令             |
| ----------------- | -------------------- | -------------------- |
| `Win + grave`     | 顯示「工作空間預覽」 | `Overview=`   |


> 關於「grave」指的是「`」，也就是「~」那個按鍵，通常在「`Tab`」上方那個按鍵。


* [設定片段: ~/.config/kglobalshortcutsrc](https://github.com/samwhelp/lubuntu-lxqt-with-kwin-adjustment/blob/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/kglobalshortcutsrc#L60)

``` sh
Overview=Meta+`,Meta+W,Toggle Overview
```

> 另外也可以直接執行「`Alt + a`」切換到「上一個工作空間」。

> 另外也可以直接執行「`Alt + s`」切換到「下一個工作空間」。




## 切換「顯示目前工作空間的所有視窗預覽」

| 按鍵組合           | 功能                                     | 執行指令             |
| ------------------ | ---------------------------------------- | -------------------- |
| `Win + Tab`        | 切換「顯示目前工作空間的所有視窗預覽」   | `Expose=`            |


* [設定片段: ~/.config/kglobalshortcutsrc](https://github.com/samwhelp/lubuntu-lxqt-with-kwin-adjustment/blob/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/kglobalshortcutsrc#L48)

``` sh
Expose=Ctrl+F9\tMeta+Tab,Ctrl+F9,Toggle Present Windows (Current desktop)
```
