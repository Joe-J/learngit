# Git clone失败 443 10054

重点
```bash
git config --global http.sslVerify "false"
```


```bash
# 取消代理
git config --global --unset http.proxy
git config --global --unset https.proxy
```
修改 hosts配置
C:\Windows\System32\drivers\etc\hosts
```
104.24.121.209 kingfast.cc
104.24.120.209 kingfast.cc
104.24.121.209 kingfast.cc
104.24.120.209 kingfast.cc

192.30.255.112 github.com git
185.31.16.184 github.global.ssl.fastly.net
140.82.114.3 github.com
151.101.1.194 github.global.ssl.fastly.net
151.101.65.194 github.global.ssl.fastly.net
151.101.129.194 github.global.ssl.fastly.net
151.101.193.194 github.global.ssl.fastly.net
```

```bash
#刷新dns
ipconfig /flushdns
```