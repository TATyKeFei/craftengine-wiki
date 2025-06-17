# Skript 教程

Skript 以下将简称 sk，CE 已经兼容了 SK

不说介绍什么的废话了直接开干！

## 物品

<!-- tabs:start -->

#### **介绍**

物品的 id 为 "<命名空间>:<id>"

比如 "default:topaz"

#### **示例代码: 进服给菜单**

```
on script load:
    set {menu} to the custom item with id "namespace:menu"

on join:
    if player does not have {menu}:
        give player {menu}
```

<!-- tabs:end -->

## 方块

> {docsify-updated}