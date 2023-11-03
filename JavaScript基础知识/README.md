# JavaScript基础知识

## Hello, world

### “script” 标签

可以在html的script标签编写js脚本

``` html
<!DOCTYPE HTML>
<html>

<body>

  <p>script 标签之前...</p>

  <script>
    alert('Hello, world!');
  </script>

  <p>...script 标签之后</p>

</body>

</html>
```

### 外部脚本

引入外部JavaScript文件

``` html
<!DOCTYPE HTML>
<html>

<body>

  <p>script 标签之前...</p>

 <script src="/path/to/script.js"></script>

  <p>...script 标签之后</p>

</body>

</html>
```

## 代码结构

### 语句

通常每行代码独占一行，尾部分号可以省略

```javascript
alert('Hello');
alert('World');
```

### 注释

```javascript
//单行注释
alert('Hello');
alert('World');
/**
 * 多行注释
 */
```

## 现代模式，"use strict"

修改js文件编写模式,通常是在文件的顶部，严格模式

```javascript
"use strict"
//编写你的JavaScript代码
```

## 变量

任何值都可以用变量来存储

### 声明

使用`let`,`var`关键字进行声明一个变量.

> 在大括号中的就属于一个块级，`{let num = 0;}`外部是无法反问的。`let`是无法重复声明一个变量的。

```javascript
//let是带有块级作用域
let num;
//var没有块级作用域
var conut = 0;
//同时声明多个变量,已逗号分隔
let num2 = 0,
    conut = 2;
{
  //只作用域{}中
  let arr = 0
}
let arr = 0
```

### 赋值

通过等号进行给变量赋值

```javascript
//声明了一个num变量并赋值给123的值
let num = 123;
//调用声明好的变量
console.log(num)//123
```

### 变量命名

- 变量名称必须仅包含字母、数字、符号 `$` 和`_`
- 首字符必须非数字。

### 保留字

不能使用这些关键字来命名变量：
比如，`let`、`class`、`return`、`function` 都被保留了。

### 常量

声明后赋值，后续无法在次修改值。声明关键字：`const`

```javascript
const conu = 100;
conu =200//这样会报错，常量是固定无法后续在次修改
```

### 大写形式的常数

使用大写字母和下划线来命名这些常量。

```javacript
const COLOR_RED = "#F00";
const COLOR_GREEN = "#0F0";
const COLOR_BLUE = "#00F";
const COLOR_ORANGE = "#FF7F00";
```

## 数据类型

js中有8种基本类型,我们可以将任何类型的值存储在一个变量中

### Number 类型

没有双引号，且全是数字。
数字可以进行一些运算：乘法 `*`、除法 `/`、加法 `+`、减法 `-` 等等。

```javascript
let count = 121212;
```

### BigInt 类型

尾部的 "n" 表示这是一个 BigInt 类型,可以存储超大数字值。

```javascript
// 尾部的 "n" 表示这是一个 BigInt 类型
const bigInt = 1234567890123456789012345678901234567890n;
```

### String 类型

所有用引号包裹的值都是字符串

- 双引号："Hello".
- 单引号：'Hello'.
- 反引号：`Hello`.

```javascript
let str = "Hello";
let danStr = 'Hello';
let newStr = `Hello`;
```

反引号可以直接在里面添加变量语法格式`helo${变量名}`

```javascript
let str = "Hello";
let danStr = 'Hello';
//拼接了danStr的值
let newStr = `Hello${danStr}`;
//可以在${}中进行运算
let newStr = `Hello${1+2}`;
```

### Boolean 类型（逻辑类型）

它只有两个值，`true`,`false`,即：真和假

```javascript
let str = "Hello";
let danStr = 'Hello';
//拼接了danStr的值
let newStr = `Hello${danStr}`;
//可以在${}中进行运算
let newStr = `Hello${1+2}`;
```

## 交互：alert、prompt 和 confirm

## 类型转换

## 基础运算符，数学运算

## 值的比较

## 条件分支：if 和 '?'

## 逻辑运算符

## 空值合并运算符 '??'

## 循环：while 和 for

## "switch" 语句

## 函数

## 函数表达式

## 箭头函数，基础知识

## JavaScript 特性
