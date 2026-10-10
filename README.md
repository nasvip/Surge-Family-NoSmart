# Surge-Family-NoSmart

「深巷有喵」[Surge-Family](https://github.com/Rabbit-Spec/Surge/blob/Master/Conf/Spec/Surge-Family.conf) 配置的**免订阅修改版**。

## 改动说明

原配置使用了 12 个 `smart` 策略组（Surge 订阅制付费功能），无订阅用户无法加载。

本版本将以下策略组全部由 `smart` 改为 **`select`（手动选节点）**，其余参数（`include-other-group`、`policy-regex-filter` 等）原样保留：

- 主力香港 / 美国 / 日本 / 台湾 / 韩国 / 新加坡节点（来自 ✈️ 主力机场）
- 备用香港 / 美国 / 日本 / 台湾 / 韩国 / 新加坡节点（来自 🚀 备用机场）

## 使用方法

1. 将文件中 `✈️ 主力机场`、`🚀 备用机场` 的 `policy-path=你的订阅地址` 替换为你自己的机场订阅链接（用不上的机场组可直接删除对应组及引用）。
2. 在 Surge 中导入本配置即可，所有地区节点组均为手动选择。

## 文件

- `Surge-Family.conf` — 修改后的完整配置
