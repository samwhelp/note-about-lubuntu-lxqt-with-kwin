---
title: 如何安裝「嘸蝦米輸入法」
nav_order: 3201
has_children: false
parent: fcitx5
grand_parent: 輸入法
---


# 如何安裝「嘸蝦米輸入法」

> 如何安裝「[fcitx5-table-boshiamy](https://packages.ubuntu.com/noble/fcitx5-table-boshiamy)」




## 微調腳本

| 微調腳本 | 中文輸入法 |
| -------- | ---------- |
| [fcitx5-table-boshiamy 安裝設定腳本](https://github.com/samwhelp/lubuntu-lxqt-with-kwin-adjustment/tree/main/prototype/main/im-config/fcitx5/fcitx5-table-boshiamy) | 嘸蝦米輸入法 |


## 指令安裝

執行下面指令，安裝「im-config」。

``` sh
sudo apt-get install im-config
```

執行下面指令，安裝「fcitx5」。

``` sh
sudo apt-get install fcitx5
```

執行下面指令，安裝「[fcitx5-table-boshiamy](https://packages.ubuntu.com/noble/fcitx5-table-boshiamy)」和「[fcitx5-chinese-addons](https://packages.ubuntu.com/noble/fcitx5-chinese-addons)」。

``` sh
sudo apt-get install fcitx5-table-boshiamy fcitx5-chinese-addons
```

執行下面指令，確保安裝支援「GTK」和「QT」環境所需要的「Package」。

``` sh
sudo apt-get install fcitx5-frontend-gtk2 fcitx5-frontend-gtk3 fcitx5-frontend-gtk4 fcitx5-frontend-qt5 fcitx5-frontend-qt6
```

執行下面指令，安裝「圖形設定介面」的「輔助工具」。

``` sh
sudo apt-get install fcitx5-config-qt
```

> 可以參考我的「[package-list.txt](https://github.com/samwhelp/lubuntu-lxqt-with-kwin-adjustment/blob/main/prototype/main/im-config/fcitx5/fcitx5-chewing/package-list.txt)」

| Package |
| ------- |
| [im-config](https://packages.ubuntu.com/noble/im-config) |
| [fcitx5](https://packages.ubuntu.com/noble/fcitx5) |
| [fcitx5-table-boshiamy](https://packages.ubuntu.com/noble/fcitx5-table-boshiamy) |
| [fcitx5-chinese-addons](https://packages.ubuntu.com/noble/fcitx5-chinese-addons) |
| [fcitx5-config-qt](https://packages.ubuntu.com/noble/fcitx5-config-qt) |
| [fcitx5-frontend-gtk2](https://packages.ubuntu.com/noble/fcitx5-frontend-gtk2) |
| [fcitx5-frontend-gtk3](https://packages.ubuntu.com/noble/fcitx5-frontend-gtk3) |
| [fcitx5-frontend-gtk4](https://packages.ubuntu.com/noble/fcitx5-frontend-gtk4) |
| [fcitx5-frontend-qt5](https://packages.ubuntu.com/noble/fcitx5-frontend-qt5) |
| [fcitx5-frontend-qt6](https://packages.ubuntu.com/noble/fcitx5-frontend-qt6) |

上面的安裝指令，可以合併在一起如下

``` sh
sudo apt-get install \
	im-config \
	fcitx5 \
	fcitx5-table-boshiamy \
	fcitx5-chinese-addons \
	fcitx5-frontend-gtk2 \
	fcitx5-frontend-gtk3 \
	fcitx5-frontend-gtk4 \
	fcitx5-frontend-qt5 \
	fcitx5-frontend-qt6 \
	fcitx5-config-qt

```




## 切換輸入法架構

執行下面指令，將「輸入法架構」切換到「fcitx5」

``` sh
im-config -n fcitx5
```

> 重新登出，然後登入，就會生效


## 加入輸入法

透過「圖形操作介面程式(`fcitx5-configtool`)」，

加入「嘸蝦米輸入法(`fcitx5-table-boshiamy`)」這個「輸入法」。




## 備註

### ~/.xinputrc

上面的步驟「`im-config -n fcitx5`」，會儲存在「~/.xinputrc」，這個檔案。

執行下面指令，觀看「~/.xinputrc」這個檔案的內容

``` sh
cat ~/.xinputrc
```

顯示

```
# im-config(8) generated on Tue, 24 May 2022 13:19:25 +0800
run_im fcitx5
# im-config signature: 1584e859fcc6846c2f86d354c758ca0e  -
```

主要是「`run_im fcitx5`」這一行。




## 相關議題

| 相關議題 |
| --- |
| [如何簡易安裝「fcitx5-table-boshiamy」](https://samwhelp.github.io/note-about-ubuntu/read/subject/im/fcitx5/howto/install-fcitx5-table-boshiamy.html) |
