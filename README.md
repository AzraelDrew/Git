```shell
#用户配置
git config --global user.name "你的名字"
git config --global user.email "你的邮箱"
```

```shell
#生成密钥
ssh-keygen -t rsa -C "你的邮箱"  然后一直回车
```

```shell
#验证
 ssh -T git@github.com
```

```shell
#设置仓库地址
git remote add 本地仓库名称 你的仓库地址
```

```shell
#修改仓库名称
git remote rename <原仓库名称> <新仓库名称>
```

```shell
#修改仓库地址
git remote set-url <本地仓库名称> <仓库地址>
```

```shell
#如果当前分支与多个主机存在追踪关系，则可以使用-u 选项指定一个默认主机，这样后面就可以不加任何#参数使用 
git push
git push -u origin master
```

```shell
#删除远程文件或文件夹
git rm -r --cached "路径+文件名"
git add .
git commit -m "delete file"
git push
```
```shell
#覆盖本地文件
git fetch --all 
git reset --hard origin/main
git pull
```
