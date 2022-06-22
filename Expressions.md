# Expressions and Operators

**An expression** is a phrase(фрагмент или фраза) of JavaScript that a JavaScript interpreter can evaluate to produce a value.(вычислить чтобы вернуть значение)

**The simplest expressions**, known as **primary expressions**, are those that stand alone—they do not include any simpler expressions.

A variable name is also a simple expression that evaluates to whatever value has been assigned to that variable.    
Reserved words like true, false, null, and this are primaryexpressions  

## Initializers  

Object and array initializers are expressions whose value is anewly created object or array.  
These initializer expressions are sometimes called **object literals** and **array literals.**  

Unlike true literals, however, they are **not primary expressions**, because they include a number of subexpressions that specify property and element values.

## Property Access  

A property access expression evaluates to the value of an object property or an array element. JavaScript defines two syntaxes  
for property access:  
expression . identifier  
expression [ expression ]

![Screenshot_4](https://user-images.githubusercontent.com/66359081/175027143-b0914d64-8d17-4263-89a4-a5239a4c77d2.png)

If the property name is a reserved word or includes spaces or punctuation characters, or when it is a number (for arrays), you  
must use the square bracket notation. Square brackets are also used when the property name is not static but is itself the result of a computation.

## Optional chaining (?.)

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Optional_chaining  
**The optional chaining** operator (?.) enables you to read the value of a property located deep  
within a chain of connected objects without having to check that each reference in the chain is valid.
