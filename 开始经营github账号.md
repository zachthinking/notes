## 简介
本文面向国内的Windows用户，介绍如何使用with-env切换代理，提交代码到github。

## 正文

如何注册github账号，如何使用github，我就不说了。

这里说一下如何提交代码或文章到github上。

假定你已经有socks5代理。

根据这篇[科学上网指南](https://github.com/haoel/haoel.github.io) 里提到的[代理技巧](https://github.com/haoel/haoel.github.io#10-%E4%BB%A3%E7%90%86%E6%8A%80%E5%B7%A7) 。

对于Windows用户，到[with-env网站](https://github.com/hellojukay/with-env) ，找到下载链接，下载最新版的`with-env_windows_amd64.exe`。
把它改名为`with-env.exe`。保存到`C:\Bin`目录下。
记得把 `C:\Bin` 加到环境变量`Path`里。

配置`~/.env`文件。

如
```
https_proxy=http://127.0.0.1:7890
http_proxy=http://127.0.0.1:7890
no_proxy=localhost,127.0.0.1

HTTPS_PROXY=http://127.0.0.1:7890
HTTP_PROXY=http://127.0.0.1:7890
NO_PROXY=localhost,127.0.0.1
```

接下来就可以愉快地使用这些命令来克隆仓库、提交代码或文章了。

```
with-env git clone ...
with-env git push ...
```
