# VPN Config

sing-box 配置 + 本体，6 条 VMess 节点 + 自动故障切换。

## 快速开始

### macOS (Apple Silicon)
```bash
chmod +x sing-box-macos-arm64
./sing-box-macos-arm64 run -c mac-config.json
# 代理: socks5://127.0.0.1:7891
```

### Windows
```cmd
sing-box-windows.exe run -c config.json
:: 代理: socks5://127.0.0.1:7890
```

## 文件

| 文件 | 说明 |
|------|------|
| `sing-box-macos-arm64` | macOS Apple Silicon 二进制 (v1.13.13) |
| `sing-box-windows.exe` | Windows x64 二进制 (v1.13.13) |
| `config.json` | Windows 配置 |
| `mac-config.json` | macOS 配置 |
| `config.json.bak` | Windows 配置备份 |

## 节点

- 🇯🇵 jp-free — 日本 (TLS)
- 🇸🇬 sg-vip1 / sg-vip2 — 新加坡
- 🇯🇵 jp-cn2-a / jp-cn2-b — 日本 CN2
- 🇬🇧 free-uk — 英国免费

## 自动切换

urltest 每 30 秒检测所有节点，自动选最快的。
Windows 端口 `7890`，macOS 端口 `7891`。
