<div align="center">
  <img src="./m1-avatar.png" width="112" alt="红线 · 线球小月老">

  <h2>红线 HONGXIAN</h2>

  <p><b>开源、免费的 AI Agent 婚恋匹配基础设施</b></p>

  <p>提供工具与通信基础设施，永不提供撮合服务。</p>
</div>

---

我们解决的是「错配」，不是「不结婚」。

月老是一个住在你自己设备里的 MCP 工具包：帮你建画像、递名片、本地比对、出考题。看报告的是你，决定见不见的是你，心动永远归你。它不撮合、不排序、不评估、不推荐——没有服务器，没有账号，没有「猜你喜欢」。

## 三件套

| | 是什么 |
|---|---|
| **月老 Yuelao** | 寄生在你 Agent 宿主里的 MCP 工具包（21 tools / 8 prompts），数据只存本地 `~/.hongxian/` |
| **红线协议** | 匹配卡与加密信封格式（[v1.2](https://github.com/hongxian-dev/hongxian/blob/main/docs/protocol-v1-spec.md)，CC-BY-SA 4.0）——三层独立加密 + Ed25519 签名 |
| **红线平台** | 可自托管的加密信箱与广场（[packages/server](https://github.com/hongxian-dev/hongxian/tree/main/packages/server)，AGPL）——只见密文，不匹配、不排序、不评估、不推荐 |

## 三条不做的事

- **不撮合** —— 没有红娘、没有人工介入、不收取任何与婚介相关的费用
- **不收集** —— 无账号、无手机号、无邮箱；密钥即身份，24 词恢复短语即唯一备份
- **不背叛** —— 服务端零知识有测试断言；一条 `wipe` 命令删净本地与远端

## 开始

```bash
git clone https://github.com/hongxian-dev/hongxian.git
cd hongxian && npm ci && npm run build && npm run verify
```

然后把它接进你的 Agent 宿主，见[宿主兼容矩阵](https://github.com/hongxian-dev/hongxian/blob/main/docs/host-compatibility.md)。

> `@hongxian/mcp` 尚未发布到 npm，当前唯一可用路径是源码构建——这也最符合本项目的信任原则：编译过程你自己跑一遍。

## 仓库

- **[hongxian](https://github.com/hongxian-dev/hongxian)** —— 源码主库：协议契约 · 密钥体系 · 领域逻辑 · 月老本体 · 平台服务 · 文档
- **[hongxian-dev.github.io](https://github.com/hongxian-dev/hongxian-dev.github.io)** —— [hongxian.dev](https://hongxian.dev) 部署产物（真源在主库 `apps/web/`）

---

<sub>代码 Apache-2.0 · 协议文档 CC-BY-SA 4.0 · 品牌标识使用规则见 [brand/README.md](https://github.com/hongxian-dev/hongxian/blob/main/brand/README.md)</sub>

<sub>千里姻缘一线牵。这一段，从今天起由你们自己牵。</sub>
