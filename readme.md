# [exert-kali](https://github.com/chaosannals/exert-kali)

```bash
# 更新系统
apt-get update
apt-get upgrade
```

## WSL2

```bash
# 进入 kali
wsl -d kali-linux
```

## 工具

```bash
# 安装 Metasploit
apt-get install metasploit-framework

# 安装 dsniff ssldump
# 含 arpspoof
apt-get install dsniff ssldump

```

## /proc/sys/net/ipv4

```bash
# 查看。
cat /proc/sys/net/ipv4/<filename>

# 是否打开 IP 转发： 0 禁止； 1 转发。
echo 1 > /proc/sys/net/ipv4/ip_forward

# 数据报的生存周期（Time To Live），即最多经过多少路由器。
echo 64 > /proc/sys/net/ipv4/ip_default_ttl

# 忽略所有的ICMP ECHO请求：0 响应；1 忽略。
echo 0 > /proc/sys/net/ipv4/icmp_echo_ignore_all

# 忽略 ICMP ECHO 多播或广播：0 响应；1 忽略。
echo 1 > /proc/sys/net/ipv4/icmp_echo_ignore_broadcasts
```
