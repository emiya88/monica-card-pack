# Monica 银行卡卡面图包 · CardFaceDB

收录 CardFaceDB 在 2026-10-25 公开目录中列出的全部 **620 张卡面**，覆盖 20 个地区分类（含“全球”）、137 个“国家/地区 + 发卡机构”组合。按国家/地区、机构与卡名命名，重名项加来源编号，便于搜索与区分版本。

## 直接订阅

推荐地址：https://raw.githubusercontent.com/emiya88/monica-card-pack/main/cardfacedb-full.json

已经订阅原 12 张测试包的用户，直接在 Monica「图源订阅 → 卡面」刷新原订阅即可。原地址现在返回同一份 CardFaceDB 全量图包：

https://raw.githubusercontent.com/emiya88/monica-card-pack/main/bank-card-test.json

两个地址任选一个。不要同时订阅，以免出现两份相同目录。Monica 里原先手动填写的订阅名称可能继续显示“银行卡测试包”，可自行改名。

初次添加：在 Monica「图源订阅 → 卡面」新增，名称填“CardFaceDB 全量卡面”，链接使用推荐地址。普通网页、卡面详情页、CSV 和 ZIP 均不是订阅地址。

## 全量范围与检查

“全量”指检查时通过 CardFaceDB 无筛选“最新”目录分页可见的全部条目。本次遍历 26 页，目录 620 项，检查通过 620 项，失败 0 项。最高来源编号不等于公开卡面数量，已移除或未公开的编号不在范围内。构建完成时复核了首页条目，未发现采集期间新增导致的首页变化。

- 原图 620 张；为兼容 Monica 改用详情页提供的大尺寸预览 0 张。逐项情况见来源表。
- 每项均实际匿名 GET，不附带账号、Cookie 或 Referer；检查 HTTPS、HTTP 状态、PNG/JPEG/WebP MIME、图像完整性及完整像素解码。
- JSON 为 79,955 字节，低于 Monica 2 MiB 图源限制；620 项低于 3000 项限制。所选图片均低于或等于 12 MiB。
- 同名卡、不同版本及来源单独列出的条目均保留。若不同条目的图像内容相同，验证报告保留对应编号，不擅自删减公开目录。
- 原始图片总量约 539.4 MiB。JSON 只包含名称和链接；Monica 加载目录后会按使用情况请求图片。

这是 2026-10-25 的人工更新快照，未启用定时更新。图片由 CardFaceDB 原站提供，未镜像到本仓库；站点调整、删除或网络状况仍可能影响后续访问。全量包尚待用户手机内确认；此前 12 张测试包已由用户确认可用。

## 文件与追溯

- `cardfacedb-full.json`：当前全量订阅。
- `bank-card-test.json`：原订阅地址的兼容副本，内容与全量订阅一致。
- `sources.csv`：每项卡名、机构、地区、详情页、原图链接、实际采用链接、尺寸、格式和哈希。
- `cardfacedb-verification.json`：目录覆盖、逐图下载、解码、体积及失败项检查记录。
- `archive/cardskin-test-12.json`：已归档的原 CardSkin 12 张测试包。
- `archive/cardskin-test-sources.csv`：原测试包的来源记录。

下载版另外提供完整 `catalog.json`、订阅地址文本和 ZIP；ZIP 本身不能用于 Monica 图源订阅。

## 来源和权利说明

素材与卡片信息来源：[CardFaceDB](https://cardfacedb.com/)。[服务条款](https://cardfacedb.com/terms.php)和[免责声明](https://cardfacedb.com/disclaimer.php)明确保留素材权利，展示或下载可用不代表授予使用或再分发许可。本仓库仅整理可访问链接与来源，未取得或宣称第三方卡面的开放许可；请依据你已具备的权利或合法依据使用，不作商业授权承诺。卡面设计与标识的权利仍归各自权利人。

格式依据：[Monica 图源订阅说明](https://github.com/Monica-Pass/Monica/blob/main/Monica%20for%20Android/docs/IMAGE-SUBSCRIPTIONS-1.0.315.zh-CN.md)。
