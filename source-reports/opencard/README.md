# OpenCard DB 可用卡面订阅

快照时间：2026-10-25T09:05:48.392451+00:00

已检查全库 548 张卡片资料；其中 233 项提供真实图片链接。实际下载并完整解码通过 208 项，合并相同 URL 后订阅图片 206 张。该合集覆盖本次验证可用的图片，不宣称覆盖缺图或不可访问的条目。

## 订阅地址

- https://raw.githubusercontent.com/emiya88/monica-card-pack/main/opencard-full.json（206 张）

在 Monica「图源订阅 → 卡面」添加以上地址。多包时逐个添加。

## 范围与验证

完整读取官方导出的全部 548 张卡片资料。源站未提供卡面的 315 项不使用占位图；对所有 233 个真实图片候选逐项 GET 和解码，208 项兼容图片通过，25 项因不可访问或格式不兼容而排除。具体原因见 excluded-unusable-images.json；缺图清单见 excluded-no-artwork.json。本包是全库中当前可匿名访问、可由 Monica 解码的图片合集，不宣称覆盖源站没有图片的条目。

图片格式：{'PNG': 156, 'JPEG': 15, 'WEBP': 37}。同内容图片按来源条目保留；完全相同 URL 按 Monica 的去重行为合并。

所有图片通过不附带账号、Cookie 或 Referer 的 HTTPS GET、响应类型、格式完整性、完整像素解码和 12 MiB 限制检查。JSON 已重新解析并检查大小、名称与地址。
图包是名称和链接索引；图片仍由原站提供。本快照没有自动更新任务，未在手机上实测新包。

## 来源与使用范围

资料来源：https://github.com/thedavidweng/opencard-db ，官方数据导出 exports/cards-all.json。资料按 CC BY 4.0 许可，须署名；代码 MIT 与资料许可均不覆盖发卡机构图片。图片版权和 attribution 属于相应发卡机构等权利人，镜像仅作识别用途，详见项目 images/README.md。本包保留来源与 attribution，只整理链接，不重新上传或转换第三方图像。

sources.csv 为逐项来源；verification.json 为完整验证记录。

其中 10 项改用存档链接明确引用的银行现行图片原址；已检查当前图片可用性，未核实与历史存档版本逐像素相同。原始存档链接和替代说明保留在验证记录中。
