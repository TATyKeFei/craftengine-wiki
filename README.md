# CraftEngine wiki (非官方)

本网站内容为 MC服务端 CraftEngine 插件的非官方用户编写的wiki

为什么有 官方Wiki 还来个 民间Wiki？ 

个人兴趣，此文档大多数为编写者使用学习时留下的笔记，希望能帮助新入坑有基础的同行

当插件有大量重构或超过两三个月没更新时请以 官方Wiki 为准

# 关于 CraftEngine​

> 搬了 minebbs 发布页面的介绍帖子

CraftEngine 重新定义了 Minecraft 插件架构，作为下一代自定义内容实现的解决方案。通过 JVM 级别的注入，它提供了前所未有的性能、稳定性和可扩展性。该框架提供了一个代码优先的 API，用于注册原生集成的方块行为和物品交互逻辑。
技术概述​

## 技术概览

### ⚙️ 方块​

CraftEngine 使用运行时字节码生成技术，在服务器原生级别注册自定义方块，并结合客户端数据包修改以实现视觉同步。此架构提供了以下功能：

### 🧱 自定义原生方块

动态注册方块，完全可控。

物理属性：硬度、引燃几率、亮度等所有标准属性

自定义行为：通过 API 实现树苗、作物、下落的方块等

原版兼容性：完全保留原版方块机制（例如音符盒、绊线）

### 📦 数据包集成

定义自定义矿脉。

生成自定义树木。

配置自定义地形生成。

### ⚡ 性能优势

比传统的 Bukkit 事件监听器更快、更稳定。

策略性代码注入以最小化开销。

# 相关链接

| 网站                 | 链接                                                              | 备注                                            |
| :---                 | :---                                                             | :---                                            |
| 原版Wiki             | https://mo-mi.gitbook.io/xiaomomi-plugins/craftengine            | 由于傻逼Gitbook的原因，国内经常上不去是正常的      |
| 汉化原版Wiki         | https://momi.gtemc.cn/craftengine                                 | 虽然普遍落后原版几个版本                         |
| Github 插件开源仓库   | https://github.com/Xiao-MoMi/craft-engine                        | 别问为什么开源还收费，有脑子都问不出这种问题        |
| modrinth             | https://modrinth.com/plugin/craftengine                          | CE 社区版发布页面                                |
| MineBBS              | https://www.minebbs.com/resources/craftengine.11281/             | 中文搬运帖子，同步[更新日志](https://www.minebbs.com/resources/craftengine.11281/updates) |
| 爱发电               | https://afdian.tv/a/xiaomomi                                     | 国内插件购买链接                                  |
| Polymart             | https://polymart.org/product/7624/craftengine                    | 在爱发电购买后可找默米给予 polymart 下载权限。不过真想吐槽国内访问 polymart 真慢下载插件也慢 |

# 不同版本间区别

| 版本              | 说明                                                                                     |
| :---             | :---                                                                                     |
| 社区版            | 仅正版服务器使用，供小型服务器、体验测试、创作者等使用                                        |
| Github 开源版本   | 所有代码开源，但需要自行构建插件jar文件                                                     |
| 付费版            | 可加入官方DC频道、QQ售后群服务第一时间反馈解答问题、获得插件jar文件，或者吹水吹牛逼             |

# 如何购买插件本体？

国内支付方式：[爱发电](https://afdian.tv/a/xiaomomi)

国外支付方式: [Polymart](https://polymart.org/product/7624/craftengine)

> {docsify-updated}