#####ssh密钥对
```bash
ssh-keygen -t rsa -C "853885165@qq.com"
cat ~/.ssh/id_rsa.pub
```
将密钥对放到github上。

#####添加远程库
github上创建远程仓库: [git_test](https://github.com/lovehhf/git_test)

    git remote add origin https://github.com/lovehhf/git_test
    or
    git remote add origin  git@github.com:lovehhf/git_test

提示:
    
    fatal: remote origin already exists.

解决:
    
    git remote rm origin

把本地库的所有内容同步到远程库上:

    git push -u origin master