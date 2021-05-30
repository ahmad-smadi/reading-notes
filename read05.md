# Reflection and Discussion

## Expressions and operators

### Operators

JavaScript has the following types of operators. This section describes the operators and contains information about operator precedence.

 #### Assignment operators
 An assignment operator assigns a value to its left operand based on the value of its right operand. The simple assignment operator is equal (=), which assigns the value of its right operand to its left operand. That is, x = y assigns the value of y to x.
#### Comparison operators
A comparison operator compares its operands and returns a logical value based on whether the comparison is true. The operands can be numerical, string, logical, or object values. Strings are compared based on standard lexicographical ordering, using Unicode values. In most cases, if the two operands are not of the same type, JavaScript attempts to convert them to an appropriate type for the comparison. This behavior generally results in comparing the operands numerically. The sole exceptions to type conversion within comparisons involve the === and !== operators, which perform strict equality and inequality comparisons. These operators do not attempt to convert the operands to compatible types before checking equality
#### Arithmetic operators
An arithmetic operator takes numerical values (either literals or variables) as their operands and returns a single numerical value. The standard arithmetic operators are addition (+), subtraction (-), multiplication (*), and division (/). These operators work as they do in most other programming languages when used with floating point numbers (in particular, note that division by zero produces Infinity).
#### Bitwise operators
A bitwise operator treats their operands as a set of 32 bits (zeros and ones), rather than as decimal, hexadecimal, or octal numbers. For example, the decimal number nine has a binary representation of 1001. Bitwise operators perform their operations on such binary representations, but they return standard JavaScript numerical values.
#### Logical operators
Logical operators are typically used with Boolean (logical) values; when they are, they return a Boolean value. However, the && and || operators actually return the value of one of the specified operands, so if these operators are used with non-Boolean values, they may return a non-Boolean value
#### String operators
In addition to the comparison operators, which can be used on string values, the concatenation operator (+) concatenates two string values together, returning another string that is the union of the two operand strings.
#### Conditional (ternary) operator
The conditional operator is the only JavaScript operator that takes three operands. The operator can have one of two values based on a condition. The syntax is:
##### condition ? val1 : val2
If condition is true, the operator has the value of val1. Otherwise it has the value of val2. You can use the conditional operator anywhere you would use a standard operator.
#### Comma operator
The comma operator (,) evaluates both of its operands and returns the value of the last operand. This operator is primarily used inside a for loop, to allow multiple variables to be updated each time through the loop. It is regarded bad style to use it elsewhere, when it is not necessary. Often two separate statements can and should be used instead.

For example, if a is a 2-dimensional array with 10 elements on a side, the following code uses the comma operator to update two variables at once
#### Unary operators
A unary operation is an operation with only one operand.

##### delete
The delete operator deletes an object's property
##### typeof
The typeof operator returns a string indicating the type of the unevaluated operand. operand is the string, variable, keyword, or object for which the type is to be returned. The parentheses are optional.
##### void
The void operator specifies an expression to be evaluated without returning a value. expression is a JavaScript expression to evaluate. The parentheses surrounding the expression are optional, but it is good style to use them.
#### Relational operators
A relational operator compares its operands and returns a Boolean value based on whether the comparison is true.


# Loops
There is many different kinds of loops , like

## FOR
## do...while
but after all they are all doing the same thing which is repeating an action some number of times.

for statement
A for loop repeats until a specified condition evaluates to false.

for ([initialExpression]; [conditionExpression]; [incrementExpression]) statement
for example

function howMany(selectObject) { let numberSelected = 0; for (let i = 0; i < selectObject.options.length; i++) { if (selectObject.options[i].selected) { numberSelected++; } } return numberSelected; }
do...while statement
The do...while statement will keep repeating the code within the do block, until a specified condition evaluates to false .

do statement while (condition);
for example

let i = 0; do { i += 1; console.log(i); } while (i < 5);