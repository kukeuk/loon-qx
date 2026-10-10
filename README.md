# loon-qx

Loon / Quantumult X 用的分流配置，和 [kukeuk/override-rules](https://github.com/kukeuk/override-rules) 的
`convert.min.js`（mihomo 版）同一套逻辑。

| 文件 | 用途 |
| ---- | ---- |
| `loon.conf` | Loon 完整配置：策略组 + 远程规则 + 本地规则 |
| `qx.conf` | Quantumult X 完整配置：策略 + 远程/本地分流 |

## 使用

1. 把对应文件导入 App（Loon / 圈X 都支持从 URL 导入）：
   - Loon：`https://cdn.jsdelivr.net/gh/kukeuk/loon-qx@master/loon.conf`
   - 圈X：`https://cdn.jsdelivr.net/gh/kukeuk/loon-qx@master/qx.conf`
2. 在 App 里添加你的节点订阅。
3. 把节点名字填进「选择代理」策略组（只需改这一个地方），其它策略组会自动跟随。

## 更新

本仓库文件由 `override-rules` 的 `scripts/generate-clients.mjs` 自动生成，
请勿手改。mihomo 那边规则变了，这里会同步重新生成。
