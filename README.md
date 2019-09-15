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

### Switch

```
switch (expression) {
  case choice1:
    // do sth
    break;

  case choice2:
    // do sth
    break;
    
  // include as many cases as you like

  default:
    // do sth
}
```

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
你可以在定义function时定义参数的默认值。

```js
function  moveLeft(xInterval = 20) {
  this.setState(state => ({ x: state.x - xInterval }));
}
```

这个例子中，`xInterval`就是一个default parameter，默认值是20。如果在调用这个function时，没有定义xInterval的值，如下，那么`xInterval`的值就是默认值。

```js
moveLeft();
```

#### Rest parameter

### Function expression
A function expression evaluates to a function reference. 在以下例子中，`function () { alert('Something happens after a certain period.') }`就是一个function expression.

```js
setTimeout(function () {
	alert('Something happens after a certain period.')
}, 1000);
```

### Arrow function
上面的例子可以用arrow function来表示。

```js
setTimeout(() => alert('Something happens after a certain period.'), 1000);
```

Arrow function其实也就是function expression的一种表达形式，更简洁。不过，`this`在arrow function里的值与一般的function expression里的不同。

#### `This` in a arrow function

## Object
Object可解释为对象或物体，如任务。有时，object只是作为一个namespace的功能，将相关的属性和方法封装起来，形成自己的scope，类似于module. 如`Math`这个对象，将`PI`，`random`等method包起来。

有时，object的功能类似于Ruby里的hash。

所以，object可以扮演3种角色，很灵活。

- 纯粹的object， 如`person`, `date`.
- Namespace.
- Hash.

### Defining an object
下面定义一个object。

```js
const article = {
  date: '2019-02-05',
  title: 'happy new year'
};
```

## Constructor, prototype, inheritance, and class

## Module

## Others
