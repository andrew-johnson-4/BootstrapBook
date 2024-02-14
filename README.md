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
* [The `strlen` Function](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Primitive-Functions#the-strlen-function)
* [The `not` Function](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Primitive-Functions#the-not-function)
* [The `write-file` Function](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Primitive-Functions#the-write-file-function)
* [The `load-file` Function](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Primitive-Functions#the-load-file-function)

### [Chapter 3: Hello World](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Hello-World)
* [Program Layout](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Hello-World#program-layout)
* [Processing Argv](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Hello-World#processing-argv)
* [Heap Allocation of Atoms](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Hello-World#heap-allocation-of-atoms)
* [Heap Allocation of Cons Cells](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Hello-World#heap-allocation-of-cons-cells)

### [Chapter 4: User-Defined Functions](https://github.com/andrew-johnson-4/BootstrapBook/wiki/User%E2%80%90Defined-Functions)
* [First-Order Functions](https://github.com/andrew-johnson-4/BootstrapBook/wiki/User%E2%80%90Defined-Functions#what-does-a-first-order-function-look-like)
* [Passing Multiple Arguments to a Function](https://github.com/andrew-johnson-4/BootstrapBook/wiki/User%E2%80%90Defined-Functions#how-are-multiple-arguments-passed-to-a-function)
* [Higher-Order Functions](https://github.com/andrew-johnson-4/BootstrapBook/wiki/User%E2%80%90Defined-Functions#what-do-higher-order-functions-look-like)

### [Chapter 5: Tokenization](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Tokenizer)
* [The Tokenizer Function](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Tokenizer#the-tokenizer-function)
* [Tokenization by Example](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Tokenizer#tokenization-by-example)

### [Chapter 6: Parsing](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Parser)
* [The Abstract Syntax Tree](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Parser#the-abstract-syntax-tree)
* [The `parse-program` Function](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Parser#the-parse-program-function)
* [The `parse-many-expressions` Function](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Parser#the-parse-many-expressions-function)
* [The `parse-one-expression` Function](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Parser#the-parse-one-expression-function)
* [The `parse-lambda` Function](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Parser#the-parse-lambda-function)

### [Chapter 7: Code Generation](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Code-Generation)
* [The Expression Datatype](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Code-Generation#the-expression-structure)
* [The `compile-expr` Function](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Code-Generation#the-compile-expr-function)
* [Codegen `this` Expressions](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Code-Generation#codegen-this-expressions)
* [Codegen `local` Expressions](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Code-Generation#codegen-local-expressions)
* [Codegen `set` Expressions](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Code-Generation#codegen-set-expressions)
* [Codegen `match` Expressions](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Code-Generation#codegen-match-expressions)
* [Codegen `foreach-atom` Expressions](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Code-Generation#codegen-foreach-atom-expressions)
* [Codegen `foreach-char` Expressions](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Code-Generation#codegen-foreach-char-expressions)
* [Codegen `while` Expressions](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Code-Generation#codegen-while-expressions)
* [Codegen `if` Expressions](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Code-Generation#codegen-if-expressions)
* [Codegen Function Application Expressions](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Code-Generation#codegen-function-application-expressions)
* [Codegen Literal Expressions](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Code-Generation#codegen-literal-expressions)
* [Codegen `argv` Expressions](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Code-Generation#codegen-argv-expressions)
* [Codegen Cons Expressions](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Code-Generation#codegen-cons-expressions)
* [Codegen Nil Expressions](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Code-Generation#codegen-nil-expressions)
* [Codegen Variable Expressions](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Code-Generation#codegen-variable-expressions)

### [Chapter 8: Type Checking](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Type-Checking)
* [Defining a Type Context](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Type-Checking#defining-a-type-context)
* [Parsing a Type Definition](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Type-Checking#parsing-a-type-definition)
* [Enumerating Inference Cases](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Type-Checking#enumerating-inference-cases)
* [Infer Type of an Ascription](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Type-Checking#infer-type-of-an-ascription)
* [Infer Type of a Literal](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Type-Checking#infer-type-of-a-literal)
* [Infer Type of a Variable](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Type-Checking#infer-type-of-a-variable)
* [Infer Type of an Application](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Type-Checking#infer-type-of-an-application)
* [Infer Type of a Lambda](https://github.com/andrew-johnson-4/BootstrapBook/wiki/Type-Checking#infer-type-of-a-lambda)

