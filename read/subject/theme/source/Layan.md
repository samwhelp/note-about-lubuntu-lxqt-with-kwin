---
title: 佈景主題來源「Layan」
nav_order: 7031
has_children: false
parent: 佈景主題來源
grand_parent: 佈景主題
---


# 佈景主題來源「Layan」




## 主題

* [佈景主題來源](#佈景主題來源)
* [外觀設定樣式](#外觀設定樣式)




## 佈景主題來源

| 佈景主題來源 | 如何安裝 |
| ---------- | ------- |
| vinceliuice / [Layan-kde](https://github.com/vinceliuice/Layan-kde) | [如何安裝](#如何安裝Layan-kde) |
| vinceliuice / [Layan-gtk-theme](https://github.com/vinceliuice/Layan-gtk-theme) | [如何安裝](#如何安裝Layan-gtk-theme) |
| vinceliuice / [Layan-icon-theme](https://github.com/vinceliuice/Layan-icon-theme) | |
| vinceliuice / [Layan-cursors](https://github.com/vinceliuice/Layan-cursors) | |
| yeyushengfan258 / [Citrus-icon-theme](https://github.com/yeyushengfan258/Citrus-icon-theme) | [如何安裝](https://samwhelp.github.io/note-about-lubuntu-lxqt-with-kwin/read/subject/theme/source/Citrus.html#如何安裝citrus-icon-theme) |


> 搜尋：「[Layan](https://github.com/vinceliuice?tab=repositories&q=Layan)」




## 外觀設定樣式

| 外觀設定樣式 |
| ---------- |
| [Layan](https://samwhelp.github.io/note-about-lubuntu-lxqt-with-kwin/read/subject/style/recipe/Layan.html) |




## 如何安裝「Layan-kde」

執行下面指令，Clone「[Layan-kde](https://github.com/vinceliuice/Layan-kde)」

``` sh
git clone https://github.com/vinceliuice/Layan-kde.git
```

執行下面指令，切換到「Layan-kde」這個資料夾

``` sh
cd Layan-kde
```

> 執行下面指令安裝

``` sh
./install.sh
```




## 如何安裝「Layan-gtk-theme」

執行下面指令，Clone「[Layan-gtk-theme](https://github.com/vinceliuice/Layan-gtk-theme)」

``` sh
git clone https://github.com/vinceliuice/Layan-gtk-theme.git
```

執行下面指令，切換到「Layan-gtk-theme」這個資料夾

``` sh
cd Layan-gtk-theme
```

執行下面指令，觀看有那些參數可以下

``` sh
./install.sh -h
```

顯示

```
'gnome-shell' not found, using styles for last gnome-shell version available.
Usage: ./install.sh [OPTION]...

OPTIONS:
  -d, --dest DIR          Specify destination directory (Default: ~/.local/share/themes)

  -n, --name NAME         Specify theme name (Default: Layan)

  -c, --color VARIANTS    Specify theme color variant(s) [standard|light|dark] (Default: All variants)

  -l, --libadwaita        Install link to gtk4 config for theming libadwaita

  -r, --remove,
  -u, --uninstall         Uninstall/Remove installed themes

  -h, --help              Show help
```

> 執行下面指令安裝

``` sh
./install.sh
```
