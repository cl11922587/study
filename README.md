# 学习笔记

## let 与 const 命令
### let用来声明变量，并且只在let申明的代码块内有效，与var区别

例如：

{
  var a =1;
  let b=2;
}
console.log(a);//1
console.log(b);//b is defined
