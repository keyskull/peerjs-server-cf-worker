# peerjs-server-cf-worker

🏗️ **WIP** – Cloudflare Workers + Durable Objects 实现的 PeerJS 信令服务器，同时内置 PeerJS 客户端源码，方便日后高度定制化。

## 目录结构

```
├── src/                  # Cloudflare Worker 服务端（Durable Object）
├── wrangler.toml
├── client/               # PeerJS 客户端源码（基于官方，可魔改）
│   ├── lib/             # 客户端核心源码
│   └── package.json
├── package.json
└── ...
```

## 服务端

基于 [jonasgloning/peerjs-server-cf-worker](https://github.com/jonasgloning/peerjs-server-cf-worker) 的快速草稿，使用 Durable Objects 实现 WebSocket 信令。

### 部署

```bash
npm install
npx wrangler deploy
```

## 客户端

`client/` 目录包含 PeerJS 客户端源码（基于官方 v1.5.x），方便你直接修改协议、消息格式或其他逻辑。

日后如需同步官方最新代码，可以对照 `peers/peerjs` 进行 merge。

## 许可

服务端部分为自有实现；客户端源码来自 PeerJS（MIT License）。
