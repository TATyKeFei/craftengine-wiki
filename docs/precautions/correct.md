# 容易误解的坑

这里列出了一些新人可能会踩的坑，不全，欢迎来 Github 提 PR 补充

## `<image>`不是 minimessage 格式

我见过太多人把 `<image>` 误解成 minimessages 的格式了，在此纠正下！

`<image>` 不属于 minimessages 格式！这是 CE 的内部变量！

```
# 当你启用配置文件 image 下的选项后，可以使用 CE 的内部变量进行替换其他插件的消息
#
# 使用场景用于为一些不支持 minimessages 或 PlaceholderAPI 的上古乐色插件服务
# 因此请禁用不必要的功能以减轻异步线程负担或者替换现代化的插件
#
# 使用方式为: <image:[命名空间]:[id]>

image:
  illegal-characters-filter:
    anvil: true
    book: true
    chat: true
    command: true
    sign: true
  intercept-packets:
    system-chat: true
    tab-list: true
    player-info: true
    set-score: true
    actionbar: true
    title: true
    bossbar: true
    container: true
    team: true
    scoreboard: true
    entity-name: false
    armor-stand: true
    text-display: true
    item: true
```

> {docsify-updated}