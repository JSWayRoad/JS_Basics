# JS_Basics    

**ECMAScript is a scripting language specification on which JavaScript is based.**

JavaScript: pocket refernce 3rd edition - https://media.oiipdf.com/pdf/3b217f0a-c6db-41d9-8af6-08ed47d9e1a5.pdf

Application Programming Interfaces (APIs) - provide you with extra superpowers to use in your JavaScript code. 
![Screenshot_21](https://user-images.githubusercontent.com/66359081/161376093-2ebd2556-c53a-4532-81c7-72df2cbe7059.png)

**What is it?**

**JavaScript is a powerful programming language that can add interactivity to a website.**  
It was invented by Brendan Eich.  

**JavaScript is a scripting or programming language that allows you to implement complex features on web pages — every time  
a web page does more than just sit there and display static information for you to look at — displaying timely content updates,  
interactive maps, animated 2D/3D graphics, scrolling video jukeboxes, etc. — you can bet that JavaScript is probably involved.**  

JavaScript is a scripting language that enables you to create dynamically updating content, control multimedia, animate images, and pretty much everything else. (Okay, not everything, but it is amazing what you can achieve with a few lines of JavaScript code.)

JavaScript is the programming language of the Web.

JavaScript is part of the triad of technologies that all Web  
developers must learn: HTML to specify the content of web  
pages, CSS to specify the presentation of those pages, and  
JavaScript to specify their behavior

JavaScript is a case-sensitive language

**JavaScript** — мультипарадигменный язык программирования. Поддерживает объектно-ориентированный, императивный и функциональный стили.

script (сценарий) — это последовательность действий, описанных с помощью скриптового языка программирования.   

**Нужно ли компилировать js в браузере?**    
Скрипты распространяются и выполняются, как простой текст. Им не нужна специальная подготовка или компиляция для запуска.  

**Есть ли строгая типизация в js и что это такое?**  
Нет. Это означает проверку типов перед запуском программы  

JavaScript динамически типизированный язык  
статическая типизация означает проверку типов перед запуском программы,  
динамическая — проверку типов, когда программа запущена.

JavaScript является слабо типизированным или динамическим языком. Это значит,  
что вам не нужно определять тип переменной заранее. Тип определится автоматически во  
время выполнения программы. Также это значит, что вы можете использовать одну переменную для хранения данных различных типов


**Императи́вное программи́рование** — это парадигма программирования (стиль написания исходного кода компьютерной программы), для которой характерно следующее: 
в исходном коде программы записываются инструкции (команды);  
инструкции должны выполняться последовательно;  
данные, получаемые при выполнении предыдущих инструкций, могут читаться из памяти последующими инструкциями;  
данные, полученные при выполнении инструкции, могут записываться в память.  

**Основные черты императивных языков:**  
исп именованных переменных;  
исп оператора присваивания;  
исп составных выражений;  
исп подпрограмм;

**Функциона́льное программи́рование** — парадигма программирования, в которой процесс вычисления трактуется как вычисление значений функций.

**Инструкции** – это синтаксические конструкции и команды, которые выполняют действия.  
**Выражение** - фрагмент кода, в котором создаётся значение.(22 или'fdsf')
**Побочные эффекты** - инструкции, которые изменяют мир или внутреннние состояние машины.
**Окружение** (environment) - это область памяти, где записываются идентификаторы и значения из областей видимости.   

**Программирование** - это процесс создания программы, набора точных инструкций, гвоорящих компьютеру, что делать.  
**Язык программирования** - это искуственный язык, созданный для написания инструкций для компьютера.  
**Инстру́кция или опера́тор** (англ. statement) — наименьшая автономная часть языка программирования; команда или набор команд.
**Код** - это текст из которого состоит программа.  

**Методология разработки программного обеспечения** — совокупность методов, применяемых при разработки программы.  
**Паради́гма программи́рования** — стиль написания кода  
**Структу́рное программи́рование** — парадигма программирования, в основе которой лежит представление программы в виде иерархической структуры блоков.

**Идентификатор** - это имя чего-либо (какой-либо сущности).  
**линтеры** – это инструменты, которые могут автоматически проверять стиль вашего кода и вносить предложения по его улучшению.

**Что такое функциональное программирование?**  
Паради́гма программи́рования — это совокупность идей и понятий, определяющих стиль написания компьютерных программ (подход к программированию).  
Функциона́льное программи́рование — парадигма программирования, в которой процесс вычисления трактуется как вычисление значений функций  


**Что такое примеси в ООП?**  
Примесь – общий термин в объектно-ориентированном программировании: класс, который содержит в себе методы для других классов.
В JavaScript можно наследовать только от одного объекта. Объект имеет единственный [[Prototype]]. И класс может расширить только один другой класс.  
 примесь – это класс, методы которого предназначены для использования в других классах, причём без наследования от примеси.  
 https://learn.javascript.ru/mixins
 
**способs подключения скрипта на страницу?**  
непосредственно на странице  
использовании отдельного файла с расширением js.  

**Как выполняются скрипты на странице**
Когда браузер при чтении страницы встречает на ней элемент script, браузер останавливает дальнейшую  
загрузку страницы и выполняет, подключенный с помощью этого элемента  
JavaScript код. После его выполнения, он приступает к дальнейшей загрузке страницы.

Как правило, JavaScript код не участвует в формировании визуальной картинки страницы.  
Поэтому чтобы страница как можно быстрее отобразилась пользователю, сценарии JavaScript  
рекомендуется подключать в самом конце страницы перед закрывающим тегом body.   

![image](https://user-images.githubusercontent.com/66359081/140582906-36f2d266-1018-4e0a-a065-722479c3912b.png)    

**Объясните проблему сравнения с помощью (==)?**  
**Как решает эту проблему оператор строгого равенства (===)?**  
Оператор строгого равенства === проверяет равенство без приведения типов.  


**undefined** выводится при попытке доступа к:
неинициализированной переменной number;
несуществующему свойству объекта movie.year;
несуществующему элементу массива movies[3].

**В каком месте лучше подключать скрипт и почему (верх, низ, лево, право)?**  
при выполнении браузером html страницы браузер выполняет ее построчно. как только встречается js   
(например линк на файл который на 4 сек заставит браузер "висеть") он выполняется, и только после этого идет чтение  
следующей строки html. потому разумнее сначала дать браузеру выполнять все body и лишь потом заставлять выполнять js  

### Как добавить script  

Для добавления кода JavaScript на страницу используется тег 
```<script>```  
Скрипт во внешнем файле можно вставить с помощью 
```
<script src="s"></script>.
```
Польза от отдельных файлов в том, что браузер загрузит скрипт отдельно и сможет хранить его в кеше.  

**Как вы понимаете определения: унарный, бинарный, операнд??**

**Операнд** – то, к чему применяется оператор. Например, в умножении 5 * 2 есть два операнда:  
левый операнд равен 5, а правый операнд равен 2. Иногда их называют «аргументами» вместо «операндов».  
**Унарным** называется оператор, который применяется к одному операнду. Например,  
оператор унарный минус "-" меняет знак числа на противоположный  
**Бинарным** называется оператор, который применяется к двум операндам. Тот же минус существует и в бинарной форме  

Большинство операторов в JavaScript возвращают значение. Для некоторых это очевидно, например сложение + или умножение *.   
Но и оператор присваивания не является исключением. Вызов x = value записывает value в x и возвращает его.  


### Есть ли строга я типизация в js и что это такое? 

Нет. Это означает проверку типов перед запуском программы.

JavaScript динамически типизированный язык  
статическая типизация означает проверку типов перед запуском программы,  
динамическая — проверку типов, когда программа запущена.

JavaScript является слабо типизированным или динамическим языком. Это значит,  
что вам не нужно определять тип переменной заранее. Тип определится автоматически во  
время выполнения программы. Также это значит, что вы можете использовать одну переменную для хранения данных различных типов

**ShadowDom?**  
Теневой DOM («Shadow DOM») используется для инкапсуляции. Благодаря ему в компоненте есть собственное «теневое» DOM-дерево, к которому нельзя просто так обратиться из главного документа, у него могут быть изолированные CSS-правила и т.д.  
Теневой DOM – это способ создать свой, изолированный, DOM для компонента.

shadowRoot = elem.attachShadow({mode: open|closed}) – создаёт теневой DOM для elem. Если mode="open", он доступен через свойство elem.shadowRoot.Мы можем создать подэлементы внутри shadowRoot с помощью innerHTML или других методов DOM.

Элементы теневого DOM:

Обладают собственной областью видимости идентификаторовНевидимы JavaScript селекторам из главного документа, таким как querySelector,Стилизуются своими стилями из теневого дерева, не из главного документа.

Теневой DOM, если имеется, отрисовывается браузером вместо обычных потомков (light DOM). В главе Слоты теневого DOM, композиция мы разберём, делать их композицию.


**Оператор typeof** возвращает строку, указывающую тип операнда  
typeof operand  
Параметры  
operand является выражением, представляющим объект или примитив, тип которого должен быть возвращён

### Тип данных Symbol

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

**Символы имеют два основных варианта использования:**

- «Скрытые» свойства объектов. Если мы хотим добавить свойство в объект, который «принадлежит» другому скрипту или библиотеке, мы можем создать символ и использовать его в качестве ключа. Символьное свойство не появится в for..in, так что оно не будет нечаянно обработано вместе с другими. Также оно не будет модифицировано прямым обращением, так как другой скрипт не знает о нашем символе. Таким образом, свойство будет защищено от случайной перезаписи или использования.

Так что, используя символьные свойства, мы можем спрятать что-то нужное нам, но что другие видеть не должны.

- Существует множество системных символов, используемых внутри JavaScript, доступных как Symbol.*. Мы можем использовать их, чтобы изменять встроенное поведение ряда объектов. Например, в дальнейших главах мы будем использовать Symbol.iterator для итераторов, Symbol.toPrimitive для настройки преобразования объектов в примитивы и так далее. 

# New Era



## Comments  

JavaScript supports two styles of comments.

![Screenshot_1](https://user-images.githubusercontent.com/66359081/174989095-9d4fa279-3d8d-4e4e-8b1e-1c05533b7f2e.png)

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




