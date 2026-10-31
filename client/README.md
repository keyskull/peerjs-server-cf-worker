# PeerJS Client (vendored)

This directory contains the PeerJS client source code, based on the official [peers/peerjs](https://github.com/peers/peerjs) (v1.5.x).

It is placed here so you can freely modify the client protocol, message format, serialization, etc. and keep it in sync with the Cloudflare Workers server in the parent directory.

## Syncing with upstream

When you need the latest official changes:

```bash
# Example workflow
cd /tmp
git clone --depth 1 https://github.com/peers/peerjs.git
# then manually merge lib/ changes into client/lib/
```

Original license: MIT
