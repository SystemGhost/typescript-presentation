Design Goals

  Extend JavaScript for writing large apps (superset of JavaScript)
  Adds support for classes, interfaces & modules.
  Development tooling support
  Compiled JavaScript runs in any browser (or Node.js).
  Since JavaScript code is TypeScript code you can start off with JavaScript and just add some types here
    and there.

Tooling Support

  Static type checking
  Strong type inference
  Symbol-based navigation
  Statement completion / intellisense
  Code refactoring

Installation
For NPM users:
  > npm install -g typescript
Provides a command-line compiler
  > tsc source.ts

File Extensions

   ts - is the extension for source files. 
  <lid.ts - is the extension for declaration files.

Declaration Source Files

  Provide type definitions, separate from the corresponding source
  Analogous to header files in C/C++
  Can be used to describe the exported virtual TypeScript types of a JavaScript library or module 
  Gives type safety, intellisense and compile errors
  DOM and jQuery provided with TypeScript
  Write your own for any existing JavaScript library / code

Type Annotations

  Optional static typing
  Lightweight way to record the intended contract of a function or variable
  Applied using a post-fix syntax
  Syntax:
    function add(a: number, b: number) {
      return a + b;
  }
  
  Return type of the function can be inferred
  Supports optional types 

Primitive Types

  number
  bool
  string
  null
  undefined

Object Types

  class
  module
  interface 
  literal types
  Supports typed arrays

const reports: Employee[] = [];
All types are subtypes of a single top type called the <span class="single-code">Any</span> type.


Functions

  Functions are the fundamental building block of any application in JavaScript
  Layers of abstraction, mimicking classes, information hiding, and modules
  In TypeScript, while there are classes, namespaces, and modules, functions still play the key role in
    describing how to do things
  Functions has optional and default parameters
  Function can be declared using Function declaration, Function expression and Arrow function
  Can be Overloaded

Generics

  Working with any types
  Most flexible
  Allows users to consume these components and use their own types

All types are subtypes of a single top type called the <span class="single-code">Any</span> type.

Classes

  Support for ECMAScript 6 alike classes
  Methods are translated into JavaScript prototype chain - more memory efficient than using closures with
    anonymous functions
   <span class="single-code">public</span> or <span class="single-code">private</span> member accessibility
  
  Parameter property declarations via constructor
  Supports single-parent inheritance
  Derived classes make use of <span class="single-code">super</span> calls to parent

Interfaces

  Designed for development tooling support only
  No output when compiled to JavaScript
  Structural type system - interfaces are automatically implemented by any object/prototype that complies
    structurally
  Supports overload by parameter signature
  Supports implementing multiple interfaces

Modules

  Analagous to .NET namespaces
  Prevents global variable naming collisions
  Closely aligned with those proposed for ECMAScript 6
  Supports code generation targeting CommonJS and AMD module systems
  Accessibility for internal and external modules


