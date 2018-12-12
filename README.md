# 学习笔记

## 函数的扩展
### 函数参数的默认值
```
function demo(x , y = 'world'){
   console.log(x,y);
}
demo('hello'); //hello
demo('hello','world');//hello world
demo('hello','');//hello
```




