```cpp
https://blog.csdn.net/weixin_42213176/article/details/100097152
git config --global user.name "username"
git config --global user.email "email"
git init
ssh-keygen -t rsa –C "email"
public-key -> github
git remote add origin http.... //连接git仓库
[create/edit/commit file]
git push origin master
//如果遇到connection was reset
先git config --global http.sslVerify "false"
再重复上述指令
```
