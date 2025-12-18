--- 
layout: '../layouts/BaseLayout.astro'
title: 'Kit Programming Language'
description: 'A magical, high performance programming language for game development.'
---

**Kit** is a programming language designed for creating concise, high performance cross-platform applications. Kit compiles to ANSI C99, so it's highly portable; it can be used in addition to or as an alternative to C, and was designed with game development in mind.


```c
include "stdio.h";

function main() {
    var s: CString = "Hello from Kit!";
    printf("%s\n", s);
}
```

**[See more code examples here](/examples)**

**At a glance:**

* Kit has a **strong, static** type system to catch errors at compile-time.
* Kit is a **procedural language**, not object-oriented or functional; however, [traits](/examples#traits), [boxes](/examples#boxes) and [abstracts](/examples#abstracts) can simulate object-oriented interfaces and polymorphism.
* Kit **compiles to standard C**, which then compiles to native libraries or executables.
* Memory management in Kit is **manual** (no automatic garbage collection), with some convenience features to make this easier.

*Kit is pre-alpha and not all features are fully implemented; see the [roadmap on Trello](https://trello.com/b/Bn9H0fzk/kit).*

**Why you should use Kit in place of:**

| C/C++ | a higher level language |
| --- | --- |
| Modern language features: type inference, [algebraic data types](/examples#enumsalgebraic-data-types), [pattern matching](/examples#match), explicit function [inlining](/examples#inline), automatic [pointer dereferencing](/examples#pointers), [generics](/examples#generics), [implicits](/examples#implicits). | Low-level control to optimize performance: [pointers](/examples#pointers), manual memory management, no GC (but easily add your own scoped memory management strategies, including reference counting/localized GC.) |
| A more expressive type system, including [traits](/examples#traits) for polymorphism, and [abstract types](/examples#abstracts), which provide custom compile-time behavioral and type checking semantics to existing types with no runtime cost. | Metaprogramming via a typed [term rewriting system](/examples#term-rewriting); use rules to transform arbitrary expressions at compile time based on their type information. Create your own interface or DSL. |
| A sane, easy to use build system. Kit features modules, imports, and standard package structure, plus a simple but powerful build tool: manage your project via a simple YAML configuration file and `kit build`, `kit test`, or `kit run`. (coming soon...) | Zero-overhead [C interoperability](/examples#c-interoperability). Take advantage of existing C libraries without any wrappers; just include the header and directly use types/functions/variables. |

**[See more comparisons here](/comparisons)**
