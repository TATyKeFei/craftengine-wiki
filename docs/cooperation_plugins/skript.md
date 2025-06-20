# Skript 教程

Skript 以下将简称 sk，CE 已经兼容了 SK

不说介绍什么的废话了直接开干！

建议配合 [官方wiki skript 教程](https://mo-mi.gitbook.io/xiaomomi-plugins/craftengine/plugin-wiki/craftengine/compatibility/skript) 观看，本教程语法可能会随着插件更新而过时

## 物品

<!-- tabs:start -->

#### **说明**

物品的 id 为 "[命名空间]:[id]"

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

<!-- tabs:start -->

#### **说明**

暂无

#### **示例: 玩家点击自定义方块时告诉玩家**

```
暂无
```

<!-- tabs:end -->

## 调用Api

<!-- tabs:start -->

#### **说明**

需要 [skript reflect](https://github.com/SkriptLang/Skript-reflect)

可用Api: `https://github.com/Xiao-MoMi/craft-engine/tree/main/bukkit/src/main/java/net/momirealms/craftengine/bukkit/api`

#### **示例: 重载资源包时告诉全服玩家**

```
import:
    net.momirealms.craftengine.bukkit.api.event.AsyncResourcePackGenerateEvent

on AsyncResourcePackGenerateEvent:
    broadcast "正在重新构建资源包!"
```

<!-- tabs:end -->

> {docsify-updated}