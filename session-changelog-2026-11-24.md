# 会话改动日志

日期：2026-11-24  
范围：本会话在本地和 Figma 中实际做过的改动。  
原始设计文件 `AR Wallet`（`YYptLQ7axFJt2SrhF2u6JU`）只读取，没有修改。

## 没有改动的内容

- 原始设计文件中的页面、组件、变量和样式。
- 已有设计规范 JSON 的色值、字号、间距等推荐项。它们的确认状态仍是 `unconfirmed`。
- 没有新建正式 Figma 组件库，没有创建变量或样式。
- 没有提交 Git。

## Figma：个人中心实验文件

文件：`个人中心`（`ewQqq2rSUNKY59hk8IcFAb`）  
页面：个人中心 `0:1`  
链接：https://www.figma.com/design/ewQqq2rSUNKY59hk8IcFAb/个人中心

这是本会话里唯一被写入的 Figma 文件。写入的是「进行中订单」弹框，不是素材提取。

新增：

- 组件 `Button/Gold`（`11:178`）。后来把圆角改为 4，高度 32，宽 66，文案仍是「去完成」。
- 组件 `Order/InProgress`（`11:180`）。底色 `#FFF4D2` 是当时写进去的，不是原设计文件里的色。
- 画板「1 笔」`11:188`、弹框 `11:197`。
- 画板「3 笔」`11:212`、弹框 `11:221`。
- 画板「超过 3 笔」`13:199`、弹框 `13:208`。列表 `13:216` 可裁切，内有 4 行；右侧另有一条示意滚动条 `13:226`。
- 组件区放在 `11:186`。原有个人中心画面 `5:156` 和组件 `5:116` 没有覆盖。

随后按历史弹框做过的调整：

- 1 笔、3 笔弹框标题栏由灰色改为白色。
- 副标题改为左对齐。
- 小按钮圆角改为 4。

当时复盘后仍留在文件里、还没有再改的差异：弹框投影、关闭图标尺寸、正文到列表的间距、行间距、按钮字重、金额字重、状态字号与颜色、订单行底色。字体用的是该文件里可用的 Noto Sans SC，原设计稿用的是 PingFang SC。

## 本地：设计规范（会话前半段新增）

目录：`ARWallet-Design-System`

这些文件是从原设计稿反向读取后写的，数值标记为现有统计、建议或待确认，没有当成已定规范。

- `04-Design-Tokens/colors.json`
- `04-Design-Tokens/typography.json`
- `04-Design-Tokens/spacing.json`
- `04-Design-Tokens/sizing.json`
- `04-Design-Tokens/radius.json`
- `04-Design-Tokens/borders.json`
- `04-Design-Tokens/shadows.json`
- `04-Design-Tokens/icon-rules.json`
- `05-Page-References/page-inventory.json`
- `06-AI-Rules/design-rules.md`
- `06-AI-Rules/design-inconsistency-report.md`
- `06-AI-Rules/pending-confirmation.md`

`pending-confirmation.md` 文首加过一段：2026-11-24 组件库第一批未创建。这段写于素材目录出现之前，里面「还没有 01-Icons、02-Images」的说法已被后面的素材提取超过，正文 20 条确认项没有改。

会话外另有一份规划画布：

`C:\Users\78156\.cursor\projects\c-Users-78156-Desktop-UIUX\canvases\ARWallet-design-system-v0.1.canvas.tsx`

## 本地：组件库阻塞记录（未建库）

组件库任务在规范未确认时停止。写的是空索引和阻塞说明，没有 Figma 组件。

- `03-Components/component-index.json`：`status` 为 `blocked`，`components` 为空，`figmaFileKey` 为 null。
- `03-Components/component-dependencies.json`
- `03-Components/component-mapping.json`
- `03-Components/component-inventory.md`
- `06-AI-Rules/component-usage-rules.md`
- `06-AI-Rules/component-validation-report.md`

## 本地：素材库（会话后半段新增）

只新增目录和文件，没有覆盖上面的规范文件。

目录：

- `01-Icons/Navigation`
- `01-Icons/General`
- `01-Icons/Business`
- `01-Icons/Banks`
- `01-Icons/Status`（空）
- `01-Icons/Social`（空）
- `01-Icons/Unclassified`（空）
- `02-Images/Logo`
- `02-Images/Avatar`（空）
- `02-Images/Banner`
- `02-Images/Illustrations`（空）
- `02-Images/Backgrounds`（空）
- `02-Images/EmptyStates`（空）
- `02-Images/Decorations`（空）
- `02-Images/Unclassified`（空）

已写入的 27 个素材：

- 导航 13 个：首页、买入、卖出、订单、我的、任务的选中与未选中，以及启动页下载图标。
- 通用 2 个：复制、联系客服。
- 业务 1 个：奖励卡。
- 银行 3 个：PhonePe、Paytm、UPI。
- Logo 6 个：无底 A 标、带白底的 64 与 120、字标、1024 与 512 应用图标位图。
- Banner 2 个：教程插画 720×332 与 360×166。

索引导出：

- `asset-index.json`
- `asset-preview.html`
- `asset-extraction-report.md`
- `asset-duplicate-report.md`
- `asset-pending-confirmation.md`

`asset-preview.html` 写完后改过一处样式：预览图由最大 96px 改为固定 96×72、`object-fit: contain`，避免 24px 图标在页面里过小。

## 本地删除

试点阶段用整节点下载得到的 5 个文件带有多余深色底，已删除，没有进入索引：

- `01-Icons/Navigation/nav-home-a.svg`
- `01-Icons/Navigation/nav-home-b.svg`
- `01-Icons/Navigation/nav-buy-a.svg`
- `01-Icons/Navigation/nav-buy-b.svg`
- `01-Icons/Navigation/nav-order-a.png`

生成索引和预览时用过的临时脚本已删除，没有留在目录里：

- `_hash_assets.py`
- `_build_preview.py`

Banner 的一次 149 字节空导出 `banner-tutorial-export.png` 已删除。两张 Banner 和两张应用图标在下载后按尺寸改过文件名，旧文件名不再存在。

## 预览检查

预览页在 `http://127.0.0.1:8765/asset-preview.html` 打开过。格式筛到 PNG 时显示 4 / 27，搜索 `phonepe` 时显示 1 / 27，深色底可以切换。直接双击 `asset-preview.html` 也可以打开，数据写在页面内部。

## 续扫（同一天，接着素材库做）

仍然只读 `AR Wallet`。个人中心实验文件没有再改。设计规范数值和确认状态没有改。没有创建组件、变量或样式。

新写入 34 个文件，索引从 27 增到 61。预览页内嵌数据已换成这份索引。临时脚本 `_append_assets.py` 用完即删。

已落盘的新增目录内容：通用图标、业务图标、银行小标、社交图标、头像、落地页 Banner、申诉插画、192 桌面标、100px 金色应用图标。

已从 Figma 导出 SVG、但还没写成文件的，记在 `asset-pending-confirmation.md`，没有记成已入库。包括 24px 深底 App_icon、airtel、MobiKwik、Super.money、后台横版 Logo、三张空状态。

## 2026-11-25 第二轮补充

原文件仍只读。没有删已有文件，没有改设计规范，没有建组件。

新写入 5 个文件：`logo-app-dark-24.svg`、`logo-arb-admin.svg`、`bank-mobikwik.svg`、`bank-supermoney.svg`、`bank-airtel.svg`。索引现为 66。最初 27 个标为 batch-01，其余 39 个标为 batch-02。

新增 `asset-coverage.json`、`asset-coverage-report.md`、`asset-similarity.json`。预览页增加来源页面、批次、选中状态筛选，以及关联对比、扫描进度、失败和待确认区块。

卖出页 MobiKwik 和我的页面 `icon` 组确认是父级或自身隐藏，没有生成替代素材。二维码确认是通用矢量图标。
