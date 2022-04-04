# JS_under_the_hood  
https://blog.bitsrc.io/javascript-under-the-hood-632ccae06b27

A JavaScript Engine is the one which takes in our code and converts it into a machine-readable language.  
It does more of a translator work, it simply translates our JS code to a language which a computer can understand.

Chakra, Microsoft IE/Edge  
SpiderMonkey, FireFox  
**V8, Chrome**  

And if everyone comes out to create an engine, it becomes totally messed up.
So, to keep an overwatch on these engines, a standard was created called **ECMA which provides  
a specification on how to write an engine and all the features of JavaScript**. 
![Screenshot_38](https://user-images.githubusercontent.com/66359081/161602320-352af469-6ce9-406e-8025-ed0cb0283b14.png)

This is what a JS Engine will look like inside. The code that we input will pass through the following stages,  
- Parser  
- AST  
- Interpreter produces ByteCode  
- Profiler    
- The compiler produces Optimized Code


## Interpreter VS Compiler

- An Interpreter reads the code line by line and executes it immediately.  
- A Compiler reads on your entire code, does some optimization and then produces an optimized code.

![Screenshot_39](https://user-images.githubusercontent.com/66359081/161602987-b4491f79-81ef-4b97-a82f-0412e28f045f.png)

- If we give this file to an Interpreter, it reads on line by line and executes the function immediately till the loop is over.  
So it just translates the code into something which our computer can understand on the go.

- And if we give this file to a Compiler, it reads on the entire program, does some analysis of what we wanted  
to do and produces an optimized code in some other language which a machine can understand. It’s like taking X(our JS file)  
& producing Y(Optimized code that a machine can understand). And if we use an interpreter on Y(Optimized code),  
the result will be the same as it was before while interpreting X(JS Code).

![Screenshot_40](https://user-images.githubusercontent.com/66359081/161603341-a585ee2f-e5ad-491c-b117-7e88d2e69088.png)

And from the above image, byte code is just an intermediate code which still needs to be interpreted for the computer to process.  
But both the interpreter and compiler converts source code into machine code but the only difference is on how the conversion is done.

An **Interpreter** converts the source code line by line to equivalent Machine Code.  
A **Compiler** converts the entire source code to Machine Code at once.

By the time, you could have known about Babel, a JS compiler that takes in your modern JS code  
and compiles down to a browser-compatible JS Code(Older JS Version).

## Pros and Cons of Interpreter & Compiler

An interpreter has the advantage of executing the code immediately without the need of any compilation. And this may seem helpful for running JS files in the browser since we don’t want to wait. But this gets slow down when there is more JS code to interpret. Remember our little code snippet where we called a function 1000 times. In that case, the output remains the same even though the function add was called 1000 times. These kinds of situations make an interpreter slow.

But a compiler can do some optimization in such cases by replacing the loop with a single number 2 (Because we added 1 + 1 every time) as it remains the same for all the 1000 iterations. The final code that a compiler gives out will be optimized and can be executed much faster.

So, an interpreter can start executing the code immediately but it does no optimization.  
While a compiler takes time to compile the code but produces a more optimized translated code.

the V8 engine also uses next feature which name is **JIT (Just In Time)** Compiler.  
It’s a combination of both the interpreter and the compiler and most of the browsers are now implementing this feature to be faster and efficient.

![Screenshot_38](https://user-images.githubusercontent.com/66359081/161604503-08b910f4-a441-492b-baae-582fce3f3461.png)

In this process,  

1. A **Parser** is the one which identifies, analyzes and classifies various parts of our program such  
as whether is it a function? is it a variable? etc by looking on the various JavaScript Keywords.

2. **AST (Abstract Syntax Trees)** then constructs a tree-like structure based on the classification from the parser.  
There’s an AST Explorer which you can check out to know how the tree is constructed.    
https://astexplorer.net/ - for check tree.

3. The Tree is then given to the **interpreter** which then produces a ByteCode. And as we saw earlier,  
byte code is not the lowest level of code but it can be interpreted. At this stage, the browser with the help  
of the V8 engine does its work with the available byte code so that the user doesn’t need to wait.

4. On the same time, the **profiler** looks for any code optimizations and then passes the input to the compiler.  
The **compiler** produces an optimized code while the byte code is used temporarily to render things on the browser.  
And as soon as the optimized code is produced by the compiler, the temporary byte code is completely replaced by this new optimized code.

5. And hence in this way, we could use the best of both the interpreter and the compiler.  
The interpreter executes the code while the profiler looks for optimization and the compiler creates an optimized code.  
Then the byte code is replaced by the optimized code which will be a lower-level code such as a Machine Code.

This simply means that the performance is going to gradually improve at the same time not blocking any execution time.

**Note on Byte Code**
As Machine Code, a byte code cannot be understood by all the computers. It still needs a middleware like  
Virtual Machine or an Engine like Javascript V8 to interpret it to a machine-readable language.  
And that’s why our browsers can execute this byte code from the interpreter during those above said 5 stages with the help of JavaScript Engines.

**Is JavaScript an interpreted language?**  
Yes, but not completely a yes. It was once during the early stages of JavaScript when Brendan Eich first created  
the JavaScript Engine ‘SpiderMonkey’. And the engine had an interpreter to tell the browser what to do.  
But now, we just don’t have interpreters alone, we have compilers. And our code is not only interpreted  
but also compiled for optimization. So technically, it all depends on the implementation.



