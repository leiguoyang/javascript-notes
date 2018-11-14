# JavaScript notes

## Variable
变量用于存放数值以多次使用。

### Define a variable
```js
var winners = 2;
```

### Declare a variable
```js
var losers;
```

未初始化的变量的值是`undefined`.

### Naming convention
变量命名需符合以下规则。

- 以字母，`_` 或`$`开头。
- 接着可用任意的字母，数字，`_`或`$`。
- 不得使用保留词(reserved keywords)，如`break`, `case`, `delete`, `static`等。

## Statement

## Expression
A expression evaluates to a value.

### Numeric expression
A numberic expression evaluates to a number.

```js
width * width
```

### String expression
A string expression evaluates to a string.

```js
'Hello' + name
```

### Boolean expression
A boolean expression evaluates to true or false.

```js
age < 14
```

## Conditional test, if...else, loop

## Function
Function就是用来完成一定功能的代码块，既可以表示成数学意义上的函数，也可以只是完成一定的功能而已。

如一个圆的面积是半径的函数，如下。

```
size = f(r) = π * r * r
```

那现在就可以定义一个function来计算面积

```js
function size(r) {
	return Math.PI * (r * r);
}
```

以上例子中，`r`叫parameter，`size`叫function name，`return`表示返回一个值。

### Function declaration
```js
function functionName(parameter_1, parameter_2, ...restParameters) {
	// the body of the function here
}
```

### Calling a function
```js
functionName(argument_1, argument_2);
```

### Parameter

#### Default parameter

#### Rest parameter

### Function expression

### Arrow function

## Object

## Constructor, prototype, inheritance, and class

## Module

## Others
