# v2bx自动化部署

执行安装脚本：


```bash
apt-get install wget -y && wget -O setup.sh https://raw.githubusercontent.com/lisi-123/v2bx-scr/main/setup.sh && chmod +x setup.sh && ./setup.sh

```

<br>
<br>

### 说明

+ 脚本自带端口映射：UDP 35000-36000 转发到 50000 （hy2端口跳跃）

<br>

+ 自动安装warp并设置本地socks5代理，让需要的网站走warp的socks5代理

  &nbsp;&nbsp;&nbsp;可修改 route.json 和 sing_origin.json 增加或者删除走warp的网站

<br>

+ warp默认ipv4优先，如果需要ipv6优先

   &nbsp;&nbsp;&nbsp;修改 /etc/V2bX/config.json 中的 SendIP 为
  
```bash
"SendIP": "::",
```

<br>

当vps同时存在v4和v6,且v6优先时候，可能会导致安装脚本出问题

执行以下脚本可临时禁用ipv6。如果要取消对v6的禁用,重启vps即可

```bash
sudo sysctl -w net.ipv6.conf.all.disable_ipv6=1
```

<br>


xiao佬的v2bx: https://github.com/wyx2685/V2bX


<br>

科技lion脚本大全

```bash
curl -sS -O https://raw.githubusercontent.com/kejilion/sh/main/kejilion.sh && chmod +x kejilion.sh && ./kejilion.sh

```

<br>


安装脚本（去除warp的版本）：

```bash
apt-get install wget -y && wget -O setup1.sh https://raw.githubusercontent.com/bsbr57442/v2bx-scr/main/setup1.sh && chmod +x setup1.sh && ./setup1.sh

```

<br>

## 有问题联系 

[https://t.me.talkingstick233_bot](https://t.me/talkingstick233_bot)

<br>
