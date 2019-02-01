1. 使用`git remote -v`查看当前远程仓库地址，输出如下：
```
origin  git@github.com:ChinaVolvocars/dagger-reflect.git (fetch)
origin  git@github.com:ChinaVolvocars/dagger-reflect.git (push)
```


2. 添加一个别名为upstream（上游）的地址，指向之前fork的地址，命令如下：
```git
git remote add upstream https://github.com/JakeWharton/dagger-reflect.git
```

3. 使用`git remote -v`查看一下上游仓库地址是否添加成功，输出如下：

```
origin  git@github.com:ChinaVolvocars/dagger-reflect.git (fetch)
origin  git@github.com:ChinaVolvocars/dagger-reflect.git (push)
upstream        https://github.com/JakeWharton/dagger-reflect.git (fetch)
upstream        https://github.com/JakeWharton/dagger-reflect.git (push)
```

   
4. 接着输入以下几个命令：
```git
git fetch upstream
git checkout master
git merge upstream/master
```



