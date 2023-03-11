# 代理

## snap 代理设置

```bash
sudo snap set system proxy.https="http://127.0.0.1:8889"
sudo snap set system proxy.http="http://127.0.0.1:8889"
```

## ssh 代理设置

样例如下

```text
Host github.com
 HostName github.com
 User git
 IdentifyFile ~/.ssh/id_rsa
 ProxyCommand nc -v -x 127.0.0.1:7891 %h %p
```
