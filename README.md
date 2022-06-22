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


## Comments  

JavaScript supports two styles of comments.

![Screenshot_1](https://user-images.githubusercontent.com/66359081/174989095-9d4fa279-3d8d-4e4e-8b1e-1c05533b7f2e.png)






