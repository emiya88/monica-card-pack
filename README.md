# Monica 银行卡与钱包卡面图包

各来源独立订阅；来源间可能有重复卡面。图片由各原站提供，本仓库仅保存名称、图片链接和来源记录。

| 来源 | 收录条目 | 订阅地址 |
|---|---:|---|
| CardFaceDB | 620 | [cardfacedb-full.json](https://raw.githubusercontent.com/emiya88/monica-card-pack/main/cardfacedb-full.json)（620 张） |
| CardSkin | 643 | [cardskin-full.json](https://raw.githubusercontent.com/emiya88/monica-card-pack/main/cardskin-full.json)（643 张） |
| AirCards | 2602 | [aircards-full.json](https://raw.githubusercontent.com/emiya88/monica-card-pack/main/aircards-full.json)（2580 张） |

在 Monica「图源订阅 → 卡面」添加所选来源的 JSON 地址；多包时逐个添加。普通网页、CSV 和 ZIP 不是订阅地址。

原来 bank-card-test.json 订阅地址继续返回 CardFaceDB 全量包。CardSkin 等新增来源使用独立地址。

## 来源与验证说明

- [CardFaceDB 说明与使用范围](source-reports/cardfacedb/README.md)
- [CardSkin 说明与使用范围](source-reports/cardskin/README.md)
- [AirCards 说明与使用范围](source-reports/aircards/README.md)

Cardentify 当前全量包未发布：源站对本检索代理禁止抓取，需站方授权或官方完整导出。详情见 [处理状态](source-reports/cardentify/README.md)。

各包是人工更新快照，没有自动更新任务。PNG/JPEG/WebP 图片按 Monica 格式验证；每包最多 3000 项、JSON 不超过 2 MiB、图片不超过 12 MiB。

原 CardSkin 12 张测试包保留在 archive/cardskin-test-12.json。卡面权利归作者或发卡机构等权利人；各图源的资料许可与图片许可应分别核对。
