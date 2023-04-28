# 1
```
https://blog.csdn.net/weixin_42213176/article/details/100097152
git config --global user.name "[username]"
git config --global user.email "[email]"
git init
ssh-keygen -t rsa –C "email"
id_rsa
'\n'
'\n'
public-key -> github
git remote add origin http.... //连接git仓库
//至此就连接好仓库了 如果仓库里有东西不能直接push  例如仓库里有一个test.txt文件
//以下方法可以  pull 修改 push
git pull origin master
//修改test.txt内容
git add test.txt
git commit -m "update"
git push origin master
//到这里就修改并重新上传了
```
# 2
```
似乎不能随便git push origin master
要本地文件有更新的时候才可以

将pull的东西删除之后再pull好像不会出现
解决方法似乎是clone
```
# 3
```
如果在 git push origin master 时
遇到  connection was reset
先git config --global http.sslVerify "false"
再 git push origin master 就可以了
```
