# AI Hive 图片与视频生成 Dify 插件

AI Hive AIGC 模型插件让 Dify 用户通过一个 API Key 调用多种图片与视频模型，适合电商主图、商品详情页、广告 KV、海报、产品精修、换背景、带货、种草、TVC、短剧、漫剧和社交媒体素材生产。

## 工具

- **图片生成与编辑**：支持 Nano Banana Pro、GPT Image 2、Seedream 5 Lite、Nano Banana 2，以及 AI Hive 当前账户可用的其他图片模型。
- **视频生成与编辑**：支持 Seedance、MiniMax H3、HappyHorse，以及 AI Hive 当前账户可用的其他视频模型。根据模型能力，可完成文生视频、图生视频、参考视频生成、视频编辑和视频延长。
- **查询生成任务**：继续查询已提交的任务，不会重复创建任务。

## 适用场景

- 淘宝、天猫、京东、拼多多、抖音电商、抖店、小红书、快手、微信小店、1688。
- Amazon、TikTok Shop、Shopify、Shopee、Lazada、Temu、AliExpress、SHEIN、Instagram。
- 商品主图、详情页、Listing、PDP、海报、广告图、直播图片、商品精修、换背景。
- 产品视频、带货视频、种草视频、广告、TVC、UGC、短剧、漫剧、动态漫画。

## 安装与配置

1. 从 Dify Marketplace 或本地 `.difypkg` 文件安装插件。
2. 在 AI Hive 的“API 接入”中创建 API Key。
3. 打开 Dify 中的 AI Hive 服务商授权面板。
4. 粘贴以 `sk-api-` 开头的 API Key 并保存。
5. 将图片生成、视频生成或任务查询工具加入 Dify Agent、Workflow 或 Chatflow。

## 使用示例

制作电商主图时，选择“图片生成与编辑”，指定 Nano Banana Pro 或 GPT Image 2 等模型，填写商品图片提示词，并按需上传商品参考图。制作视频时，选择“视频生成与编辑”，指定可用的 Seedance 或 MiniMax 模型，填写视频提示词，并上传所选模型支持的参考素材。

## 网络要求

- 可通过 HTTPS 访问 `https://ai-hive.iclip.cn/api`。
- 拥有有效的 AI Hive API Key。
- 可访问 AI Hive 返回的生成结果地址。

AI Hive 是外部服务。模型调用可能按照用户 AI Hive 账户中显示的价格消耗付费额度；Dify 插件本身不销售订阅，也不处理付款。

插件会在执行用户请求时将提示词、生成参数和必要的参考素材发送给 AI Hive，不会在源代码中内置或记录用户的 API Key。

源码：<https://github.com/wubin1836/ai-hive-dify-plugin>

## 许可证

MIT
