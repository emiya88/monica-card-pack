# Monica 银行卡卡面测试包

12 张真实银行卡面：10 张中国卡面、2 张美国运通卡面。此仓库仅整理公开图片直链和来源信息；原图由 CardSkin 提供。

## 订阅地址

https://raw.githubusercontent.com/emiya88/monica-card-pack/main/bank-card-test.json

在 Monica 的「图源订阅 → 卡面」添加上述 HTTPS 地址。名称可填“银行卡测试包”。目录应显示 12 张，再选一张检查图片下载与裁剪。

不要订阅本仓库首页、GitHub 的文件详情页或 CardSkin 的卡面详情页。

## 内容与验证

- `bank-card-test.json`：UTF-8 JSON，顶层 `name`、`images`，每项 `name`、`url`，无占位链接。
- `sources.csv`：逐图来源页、发卡机构、原图直链、使用限制与检查记录。

2026-10-25，12 个链接均经无账号、Cookie 或 Referer 的实际 GET 检查，返回 HTTP 200、image/png，尺寸均为 1536×969。PNG 文件头、完整性、完整像素解码以及 URL 和图片内容去重检查通过。JSON 已写入后重新解析，并对照 Monica 的图源解析格式与大小限制检查。

Android Monica 内的订阅、选图和裁剪仍需用户设备确认。第三方链接可能因网络状况、站点调整或下架而失效。

## 来源与使用范围

素材来源：[CardSkin](https://cardskin.app/)。各详情页说明真实卡面供个人在自己的设备上使用，设计与商标属于发卡机构等权利人；CardSkin 与发卡机构无关联。[站点上传与下架规则](https://cardskin.app/guidelines)。逐图信息见 sources.csv。

上述依据是素材站的个人使用说明，不是已核实的发卡机构授权或开放再分发许可证。本仓库没有为第三方图像授予许可，未确认商业使用、原图镜像或大规模公开分发授权。请仅用于个人测试；公开扩展与推广前应另行取得权利人许可。

格式依据：[Monica 图源订阅说明](https://github.com/Monica-Pass/Monica/blob/main/Monica%20for%20Android/docs/IMAGE-SUBSCRIPTIONS-1.0.315.zh-CN.md)。
