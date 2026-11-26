# 组件检查

日期：2026-11-25  
没有创建或修改 Figma 组件。

## 已读到的原生组件

首页顶层确认 15 个 Component，0 个 Component Set。Key 记在 `03-Components/component-index.json`。

- 状态栏 2 个：`StatusBar_white`、`StatusBar_black`
- 导航 12 个：`icon_home1/2`、`icon_buy1/2`、`icon_sell1/2`、`icon_order1/2`、`icon_my1/2`、`icon_task1/2`
- `VIP Bonus Alert!`

复制图标 `7990:5468` 也是 Component，但这次没有读到父页面。

## 不能写成总数的部分

首页一次深层遍历在 2500 个节点处截断，遍历顺序又没走到这些顶层组件，所以那次结果里的 0 个组件、15 个实例，都不能当成全文件数量。

其他页面没有做组件普查。

## 分类

| 类型 | 本轮能确认的数量 |
| --- | --- |
| 原生 Component | 15，另有 1 个页面未定位 |
| Component Set | 抽样里是 0，不是全文件总数 |
| Instance | 未统计 |
| 组件候选项 | 看到买入页大量支付行和标志画板是 Frame，没有逐个编号 |
| 规划组件 | 0。旧索引是空的 |
| 已标准化组件 | 0 |

买入页的支付行、弹窗、登录画面目前是普通 Frame，不能记成已经创建的组件。
