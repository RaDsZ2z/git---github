# 1
```
https://blog.csdn.net/weixin_42213176/article/details/100097152
git config --global user.name "[username]"//最好是github昵称?
git config --global user.email "[email]"//最好是注册github的邮箱?
git init
ssh-keygen -t rsa –C "email"
id_rsa
'\n'
'\n'
public-key -> github
git remote add origin https.... //连接git仓库
//git remote rm origin 可以删除关联的远程库
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
在 git clone 时(git clone https://github.com/RaDsZ2z/test.git)
遇到  connection was reset
先git config --global http.sslVerify "false"
再 git push origin master 就可以了
注:使用git config --list查看http.sslVerify值本来就为false
但还是要再设置为false才可以
有说法可以使用  "git@github.com..."绕过验证 但是没有试成功
```
# 4
```
在 git push origin master 时
遇到  connection was reset
先git config --global http.sslVerify "false"
再 git push origin master 就可以了
```



