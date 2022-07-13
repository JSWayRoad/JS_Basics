## Identifiers and Reserved Words

**An identifier is simply a name**  

In JavaScript, identifiers are used  
to name variables and functions and to provide labels for certain loops in JavaScript code. A JavaScript identifier must begin  
with a letter, an underscore (_), or a dollar sign ($). Subsequent  
characters can be letters, digits, underscores, or dollar signs.

JS usually treats line breaks as semicolons only if it can’t
parse the code without the semicolons.

## Types, Values, and Variables  

The ECMAScript language types are Undefined, Null, Boolean, String, Symbol, Number, BigInt, and Object.  
https://262.ecma-international.org/12.0/#sec-ecmascript-data-types-and-values

В JavaScript есть 8 основных типов.

**number** для любых чисел: целочисленных или чисел с плавающей точкой; целочисленные значения ограничены диапазоном ±(253-1).  
**bigint** для целых чисел произвольной длины.  
**string** для строк. Строка может содержать ноль или больше символов, нет отдельного символьного типа.  
**boolean** для true/false.  
**null** Это просто специальное значение, которое представляет собой «ничего», «пусто» или «значение неизвестно», которое указано явно(явное обозн ничего)  
**undefined** Оно означает, что «значение не было присвоено» (неявное обозн ничего)  
**object** см 3 
**symbol** для уникальных идентификаторов.

**Types** are the kinds of values that can be represented and manipulated in a programming language.  

When a program needs to retain a value for future use, it assigns the value to (or “stores” the value in) a **variable**.  
A variable defines a symbolic name for a value and allows the value to be referred to by name.

JavaScript types can be divided into two categories: **primitive types** and **object types**.  
JavaScript’s primitive types include numbers, strings of text (known as strings), and Boolean truth values (known as booleans).  

JavaScript variables are untyped.  

Variables are declared with the var keyword. JavaScript uses **lexical scoping**.    
Variables declared outside of a function are **global variables** and are visible everywhere in a JavaScript program.  
Variables declared inside a function have **function scope** and are visible only to code that appears inside that function.

## Numbers  

All numbers in JavaScript are represented as floating-point values.  
When a number appears directly in a JavaScript program, it’s called a **numeric literal**.

## Text  

A **string** is an immutable ordered sequence of 16-bit values, each of which typically represents a Unicode character—
strings are JavaScript’s type for representing text.

## Boolean Values  

A boolean value represents truth or falsehood, on or off, yes or no.     
The following values convert to, and therefore work like, false: undefined null 0 -0 NaN "" // the empty string

## null and undefined  

The **undefined** value represents a deeper kind of absence. It is  
- the value of variables that have not been initialized  
- the value you get when you query the value of an object property or array element that does not exist  
- the undefined value is also returned by functions that have no return value, and the value of function parameters for which no argument is supplied.  
- ndefined is a predefined global variable (not a language keyword like null) that is initialized to the undefined value.  

**undefined** выводится при попытке доступа к:
неинициализированной переменной number;
несуществующему свойству объекта movie.year;
несуществующему элементу массива movies[3].


## Symbols  

**Символы имеют два основных варианта использования:**

- «Скрытые» свойства объектов. Если мы хотим добавить свойство в объект, который «принадлежит» другому скрипту или библиотеке, мы можем создать символ и использовать его в качестве ключа. Символьное свойство не появится в for..in, так что оно не будет нечаянно обработано вместе с другими. Также оно не будет модифицировано прямым обращением, так как другой скрипт не знает о нашем символе. Таким образом, свойство будет защищено от случайной перезаписи или использования.

Так что, используя символьные свойства, мы можем спрятать что-то нужное нам, но что другие видеть не должны.

- Существует множество системных символов, используемых внутри JavaScript, доступных как Symbol.*. Мы можем использовать их, чтобы изменять встроенное поведение ряда объектов. Например, в дальнейших главах мы будем использовать Symbol.iterator для итераторов, Symbol.toPrimitive для настройки преобразования объектов в примитивы и так далее. 

**Символ (symbol)** – примитивный тип данных, использующийся для создания уникальных идентификаторов.

«Символ» представляет собой уникальный идентификатор.  
Создаются новые символы с помощью функции Symbol():
``` 
// Создаём новый символ - id
let id = Symbol();
``` 
При создании символу можно дать описание (также называемое имя), в основном использующееся для отладки кода:
``` 
// Создаём символ id с описанием (именем) "id"
let id = Symbol("id");
``` 

**Описание** – это просто метка, которая ни на что не влияет.  
Символы не преобразуются автоматически в строки  
Символы позволяют создавать «скрытые» свойства объектов, к которым нельзя нечаянно обратиться и перезаписать их из других частей программы.  
Символы игнорируются циклом for…in

**Системные символы**
Существует множество «системных» символов, использующихся внутри самого JavaScript, и мы можем использовать их, чтобы настраивать различные аспекты поведения объектов.

Даже если символы имеют одно и то же имя, это – разные символы. Если мы хотим, чтобы одноимённые символы были равны, то следует использовать глобальный реестр: вызов Symbol.for(key) возвращает (или создаёт) глобальный символ с key в качестве имени. Многократные вызовы команды Symbol.for с одним и тем же аргументом возвращают один и тот же символ.

## The Global Object  

**The global object** is a regular JavaScript object that serves a very important purpose: the properties of this object are the globally  
defined symbols(сущности) that are available to a JavaScript program.  

When the JavaScript interpreter starts (or whenever a web browser loads a new page), it creates a new global object and  
gives it an initial set of properties that define:  
 Global properties like undefined, Infinity, and NaN  
 Global functions like isNaN(), parseInt() , and eval(.  
 Constructor functions like Date(), RegExp(), String(),  
 Object(), and Array()  
 Global objects like Math and JSON 
 
 
## Type Conversions
![Screenshot_2](https://user-images.githubusercontent.com/66359081/175017601-1593845c-224f-489d-9ab9-69fc57cb0fc0.png)
![Screenshot_3](https://user-images.githubusercontent.com/66359081/175017610-4ee8062a-ba5f-46d9-ba1a-f35311cdff4e.png)

# Variables    

A variable is a property of a special internal object, associated with the currently executing block/function/script.

## Variable Declaration  

Before you use a variable in a JavaScript program, you should declare it.

**The scope of a variable** is the region(фрагмент) of your program source code in which it is defined(в котором её можно считать определённой).  

A global variable has **global scope**; it is defined everywhere in your JavaScript code.  
variables declared within a function are defined only within the body of the function. They are local variables and have **local scope**.  
Within the body of a function, a local variable takes precedence over a global variable with the same name.

JavaScript’s function scope means that all variables declared within a function are visible throughout the body of the function.  
Curiously, this means that variables are even visible before they are declared. This feature of JavaScript is informally known as **hoisting**:  
JavaScript code behaves as if all variable declarations in a function (but not any associated assignments) are “hoisted” to the top of the functio


