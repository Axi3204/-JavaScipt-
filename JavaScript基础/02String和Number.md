# 基本数据类型 String 
## 引号的注意事项
- 单引号和单引号不能混用
- 同类引号不能嵌套，双引号里不能再放双引号
- 双引号里可以嵌套单引号，反之亦然

## 转义字符
- \r表示回车
- \n表示换行
- \t表示缩进
- \b表示空格

## 字符串的长度
> str.length
- 一个空格是一个字符
- 一个符号是一个字符
- 一个英文字母是一个字符

## 字符串拼接
> 字符串 + 任意类型的数据 = 新的字符串

## 字符串的不可变性
```js
let str = 'hello';
str =  'world';
```
字符串的值不能改变，但是可以改变字符串的地址。

## 模板运算符
```js
let a = 'this is a string';
console.log(`模板字符串${a}`);//模板字符串this is a string
```
同时模板字符串可以添加表达式
```js
const  x = 1;
const y = 2;
console.log(`${x} + ${y} = ${x + y}`);//1 + 2 = 3
```

# 基本数据类型Number
## Number的数值范围
> 最大值：Number.MAX_VALUE，这个值为： 1.7976931348623157e+308
> 最小值：Number.MIN_VALUE，这个值为： 5e-324

如果超出了这个值将会返回Infinity 
Tips: 
```js
typeof Infinity // number
```

## NaN 
NaN是一个特殊的数字，表示 Not a Number，非数值。在进行数值运算时，如果得不到正常结果，就会返回 NaN。
Tips: 
```js
typeof NaN // number
```