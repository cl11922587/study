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
### 函数的length属性
```
(function (a) {}).length // 1

(function (a = 5) {}).length // 0

(function (a, b, c = 5) {}).length // 2

如果设置了默认值的参数不是尾参数，那么length属性也不再计入后面的参数了。

(function (a = 0, b, c) {}).length // 0

(function (a, b = 1, c) {}).length // 1
```
### 一个简单的判断参数不能省略
```
function throwIfMissing() {
  throw new Error('Missing parameter');
}

function foo(mustBeProvided = throwIfMissing()) {
  return mustBeProvided;
}

foo()
// Error: Missing parameter
```




