# Local Agent MCP — Linux downloads

Bản Linux đóng gói (linux-x64). Source nằm ở repo riêng, không public.

## Tải

File mới nhất: [LocalAgentMCP-linux-x64.tar.gz](https://github.com/trunghoang0501/local-agent-releases/releases/latest/download/LocalAgentMCP-linux-x64.tar.gz)

## Cài trên server Ubuntu/Debian

```bash
curl -fsSL -o LocalAgentMCP-linux-x64.tar.gz \
  https://github.com/trunghoang0501/local-agent-releases/releases/latest/download/LocalAgentMCP-linux-x64.tar.gz
tar -xzf LocalAgentMCP-linux-x64.tar.gz
cd LocalAgentMCP-linux-x64
sudo bash install.sh
```

Script cài binary vào `/opt/local-agent` và bật systemd `local-agent.service`.

- Console: `http://<ip-server>:8787`
- MCP: `http://<ip-server>:8001/mcp` (bật Listen on LAN trong console)
- Nếu firewall chặn: `sudo ufw allow 8787/tcp && sudo ufw allow 8001/tcp`
