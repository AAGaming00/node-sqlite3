# Fork of node-sqlite3 with many pre-built supports

Mainly used for my another project - [Uptime Kuma](https://github.com/louislam/uptime-kuma)

Although the main node-sqlite3 got updated, but there is still no arm pre-built. So this fork is still needed.

- Support armv7 / arm64 pre-built
- Support Alpine (musl) pre-built
- Support Windows pre-built
- Support MacOS pre-built
- Fix worker_threads problem

PS: No electron supports

## How to use

```
npm install @louislam/sqlite3
npm remove sqlite3
```

Replace require("@louislam/sqlite") in your source code

## Prepare Prebuilt

glibc
- armv7 - npm run build-linux-arm (Support glibc >=2.18 only)
- amd64/arm64 - npm run build-linux

musl (alpine)
- armv7/arm64/amd64 - npm run build-linux-alpine

Windows / MacOS
- Get from Github Action
