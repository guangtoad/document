# Git版本管理

## 撤销一次操作
```
    git reset HEAD~1 --soft
```

## 放弃合并
```
    git merge --abort 
```

## 如何强制git pull

```
    git fetch --all
    git reset --hard origin/<branch_name>
```