# 重复素材记录

比对范围现为已经落盘的 61 个文件。没有任何两个文件的 SHA-256 相同，所以没有删除任何文件。下面第 1 到第 4 节是前 27 个文件的记录。第 5 节是续扫追加。

## 1. 字节完全相同

无。

## 2. 画面相同、文件不同

建议关联，不合并。

| 保留文件 | 关系 | 建议 |
| --- | --- | --- |
| `banner-tutorial-720.png`（720×332）与 `banner-tutorial-360.png`（360×166） | 同一教程插画的两张原图，都来自节点 `13128:6596` | 页面按 360×166 使用。不要把 360 放大成 720。 |
| `logo-app-icon-1024.png` 与 `logo-app-icon-512.png` | 同一圆角应用图标的两档原图，都来自节点 `9096:1953` | 需要位图时用对应尺寸，不要互相放大。 |
| `logo-mark-64.svg`、`logo-app-64.svg`、`logo-app-120.svg` | 同一金色 A。64 无底版没有白底；另外两份的白底在 Figma 画板里 | 透明场合用无底版。矢量可以缩放，尺寸文件仍都保留。 |
| UPI `7098:1645` | 我的页 `305:4041`、卖出页 `21049:11054` 同名 | 只保存了可导出的一份。另外两处记为来源，没有第二份文件。 |
| PhonePe `10049:2491` | 收银台另有同名框 `10049:2559` | 只保存一份。 |
| Paytm `10049:2474` | 收银台另有同名框 `10049:2576` | 只保存一份。未导出带文案的整行。 |
| 复制 `7990:5468` | 我的页实例 `7990:5475` 为 12×12 且不可见 | 保存母版。12×12 是实例缩放，不另存。 |

## 3. 选中与未选中

以下 6 对都保留，没有去重：

- nav-home-active / nav-home-inactive
- nav-buy-active / nav-buy-inactive
- nav-sell-active / nav-sell-inactive
- nav-order-active / nav-order-inactive
- nav-profile-active / nav-profile-inactive
- nav-task-active / nav-task-inactive

前 5 对主要是金色渐变和灰色的差别。任务这一对除了颜色，白色图形也不同。

## 4. 未执行的合并

外观接近但功能不同的图标没有合并。买入、卖出、订单、任务、我的各自保留。

## 5. 续扫里没有另存的来源

| 已保留文件 | 未另存的来源 | 原因 |
| --- | --- | --- |
| `business-qr.svg`（14607:4069） | 自动交易 `18638:12283` | 导出长度 6166 与 6165，同一二维码。 |
| `business-reward-type.svg` | `26558:4778` 奖励类型1_icon | 图形几乎相同。 |
| `business-order-reward.svg` | `26558:4784` 奖励类型2_icon | 图形几乎相同。 |
| `bank-upi.svg` | `305:4041` 已在来源里 | 同为 28×8 左右的 UPI，路径末位不同，不是字节相同。 |
| `banner-tutorial-720.png` | `13107:10447` | 与 720 原图哈希相同。 |
| `logo-mark-192.svg` | 无第二份 | 与 `logo-mark-64.svg` 相关，路径不是简单放大，两份都留。 |
| `bank-phonepe.svg` | `bank-phonepe-ring.svg` 另存 | 颜色和尺寸不同，不合并。节点名虽是 MobiKwik_logo 3，图形是 PhonePe。 |
| `avatar-03.jpg` | `avatar-04.jpg` 另存 | 同一人物、不同原图。 |
| `illustration-appeal-1.png` / `illustration-appeal-2.png` | 同节点子树里的较小原图另存 | 文件不同，都留，状态 unconfirmed。 |
| WhatsApp / Telegram | 26px 副本 | 是 66px 母版的缩放。 |

组合行 `26384:17470`（图层加 MobiKwik）和带文案的 Paytm 整行没有当 Logo。
