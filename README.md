# Bootstrap Book
Learn how to Write a Compiler in 2000 Lines of Code

### λ☶

[This book](https://github.com/andrew-johnson-4/BootstrapBook/wiki) explains the code of the [λ☶ compiler](https://github.com/andrew-johnson-4/-) to anyone who is interested in compiler architecture or functional language compilers.
The code is roughly 2000 LOC in length, but it is very terse, so the explanation takes a while.
The generated code is in the format of GNU Assembly for legibility.
Binary targets are just as easy to write, but harder to read.

### [Chapter 1: S-Expressions](https://github.com/andrew-johnson-4/BootstrapBook/wiki/S%E2%80%90Expressions)
* [The S-Expression Type Signature](https://github.com/andrew-johnson-4/BootstrapBook/wiki/S%E2%80%90Expressions#the-type-signature)
* [Why are S-Expressions Good](https://github.com/andrew-johnson-4/BootstrapBook/wiki/S%E2%80%90Expressions#why-are-s-expressions-good)
* [How Do We Construct An S-Expression in Assembly](https://github.com/andrew-johnson-4/BootstrapBook/wiki/S%E2%80%90Expressions#how-do-we-construct-an-s-expression-in-assembly)
* [What Common Functions Operate on S-Expressions](https://github.com/andrew-johnson-4/BootstrapBook/wiki/S%E2%80%90Expressions#what-common-functions-operate-on-s-expressions)

### [Chapter 2: Primitive Functions](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Primitive-Functions)
* [What Is a Function?](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Primitive-Functions#what-is-a-function)
* [What Do We Expect From a Function Inside the Compiler?](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Primitive-Functions#what-do-we-expect-from-a-function-inside-the-compiler)
* [System Calls](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Primitive-Functions#system-calls)
* [The `print-s` Function](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Primitive-Functions#the-print-s-function)
