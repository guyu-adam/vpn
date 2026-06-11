# VPN Config

sing-box 配置，6 条 VMess 节点 + 自动故障切换。

## 文件

| 文件 | 说明 |
|------|------|
| `config.json` | Windows 当前配置 |
| `config.json.bak` | Windows 备份 |
| `mac-config.json` | macOS 配置 |

## 节点

- 🇯🇵 jp-free — 日本 (TLS)
- 🇸🇬 sg-vip1 / sg-vip2 — 新加坡
- 🇯🇵 jp-cn2-a / jp-cn2-b — 日本 CN2
- 🇬🇧 free-uk — 英国免费

## 使用

```bash
sing-box run -c config.json
```

代理端口：Windows `127.0.0.1:7890` / macOS `127.0.0.1:7891`
