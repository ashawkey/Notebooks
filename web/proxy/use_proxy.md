# use proxy



### find the right port !!!

trojan-qt5 local client's socks port is in "入站设置", not "出站设置".

the default is `socks5://127.0.0.1:51837 `



### git

```bash
# set (do not need to set https.proxy!)
git config --global http.proxy socks5://127.0.0.1:51837 

# unset
git config --global --unset http.proxy

# show 
git config --global http.proxy 
```



### bash

```bash
# set
export http_proxy=http://10.1.3.1:8080
export https_proxy=http://10.1.3.1:8080

# unset
export http_proxy=
export https_proxy=

# show
echo $http_proxy
echo $https_proxy
```



### powershell

(not tested)

```powershell
# set
netsh winhttp set proxy "192.168.0.14:3128"

# unset 

# show
netsh winhttp show proxy
```

