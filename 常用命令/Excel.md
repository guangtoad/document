# Excel常用公式

## 获取扩展名
```
=IF(LEN(A2)-LEN(SUBSTITUTE(A2,".",""))>0,"."&MID(A2,FIND("*",SUBSTITUTE(A2,".","*",LEN(A2)-LEN(SUBSTITUTE(A2,".",""))))+1,LEN(A2)),A2)
```

## 偶去啥获取目录里面的文件名

### macOS
```
=IF(LEN(A2)-LEN(SUBSTITUTE(A2,"/",""))>0,MID(A2,FIND("*",SUBSTITUTE(A2,"/","*",LEN(A2)-LEN(SUBSTITUTE(A2,"/",""))))+1,LEN(A2)),A2)
```
### windows
```
=IF(LEN(A2)-LEN(SUBSTITUTE(A2,"\",""))>0,MID(A2,FIND("*",SUBSTITUTE(A2,"\","*",LEN(A2)-LEN(SUBSTITUTE(A2,"\",""))))+1,LEN(A2)),A2)
```