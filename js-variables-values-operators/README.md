# JavaScript Variables, Values, Types and Operators

## Objectives

* Review the JavaScript Data types
* Remember how to declare a variable
* Beware of operators results per data types


## Review

### Expression

In JavaScript an expression is anything that evaluates to a single value. 

The following is an expression that evaluates to `7`

```js
5 + 2
```

### Statements

A statement is an instruction to perform a specific action. Statements usually end with a semicolon or occupy a single line of code. Statements include `if`, `for` statements, function declarations and assigning a value to a variables

Example:

```js
let a = 90; // A variable declaration statement
if (a < 80) { // An if statement
  console.log('a is less than 80')
}
```

### Data Types

**Exercise**: List as many JavaScript data types as possible.

| Primitive                                                                      | Structural (non-primitive) |
| ------------------------------------------------------------------------------ | -------------------------- |
| undefined                                                                      | Object                     |
| Boolean                                                                        | Function                   |
| Number                                                                         |
| String                                                                         |
| [BigInt<sup>*</sup>](https://developer.mozilla.org/en-US/docs/Glossary/BigInt) |
| [Symbol<sup>*</sup>](https://developer.mozilla.org/en-US/docs/Glossary/Symbol) |

>\*not covered here. See link to resource.

#### Number

```js
typeof 42 // => 'number'
```

You all know numbers. Numbers in Javascript are stored in 64 bits. Which means that any number declared in your programs occupy 64 one and zeros in memory. This 64bits let you write number as big as -(25<sup>3</sup> − 1) and 25<sup>3</sup> − 1

##### Interesting Numbers

* `+Infinity`
* `-Infinity`
* `Number.MAX_VALUE`
* `Number.MAX_SAFE_INTEGER`
* `Number.MIN_SAFE_INTEGER`
* `NaN` (Not a Number)

##### Arithmetic Operators

* `+` Addition operator.
* `-` Subtraction operator.
* `/` Division operator.
* `*` Multiplication operator. 
* `%` Remainder operator.
* `**` Exponentiation operator.

##### Order of operations

Arithmetic operation execute just like in algebra and can be grouped with parenthesis

```js
> 2 + 2 * 4
10

> 23 * 2 - 4 / 4
45

> ((23 * 2) - 4) / 4
10.5
```

**Exercise**: In the node repl in the terminal play with some numbers and arithmetic operators.

### String

In any computer programming language, a string is a sequence of characters used to represent text.

Strings are immutable and have properties.

```js
let str = 'hello'
str[0] = 'H' // Will not change str. Immutable
str.length // Length property 5
```

#### Concatenation

The `+` operator is used for joining two or more strings strings. 

```js
'Hello ' + 'World!' // => 'Hello World'
'5' + 5 // => '55'
```

If one of the operands is a string the other one will be converted to a string and they will be joined.

**Question:** What other are common operations you do with strings.

### Boolean

Can only be one of two values: `true` or `false`. You can write the as literals or you they can be obtained from comparison or logical operations.

#### Comparison Operators

* `===` Strict Equal
* `!==` Strict not equal
* `>` Greater than
* `>=` Greater than or equal to
* `<` Less than
* `<=` Less than or equal to

Avoid using: `==` and `!=`.

#### Logical Operators

* `&&` Logical AND
* `||` Logical OR
* `!` Logical NOT

## Resources

* [JavaScript Expressions and Statements - Medium](https://medium.com/launch-school/javascript-expressions-and-statements-4d32ac9c0e74)
* [Expressions and Operators - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)
