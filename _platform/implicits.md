---
authors: [kc, yallop, avsm, fred]
title: "Modular Implicits"
layout: page
---

{% mermaid %}
graph LR;
Platform("OCaml Platform")
click Platform "/platform/index.html" "Platform"
Compiler
click Compiler "/platform/compiler.html" "Compiler"
Platform --> Compiler
Compiler --> Features
click Features "/platform/compiler-features.html" "Features"
Features --> Implicits
click Implicits "/platform/implicits.html" "Implicits"
style Implicits stroke:#000000,stroke-width:2px;
{% endmermaid %}

A common criticism of OCaml is its lack of support for ad-hoc polymorphism. The classic example of this is OCaml's separate addition operators for integers `(+)` and floating-point numbers `(+.)`. Another example is the need for type-specific printing functions (`print_int`, `print_string`, etc.) rather than a single print function which works across multiple types.

Taking inspiration from [Scala's implicits](http://docs.scala-lang.org/tutorials/tour/implicit-parameters.html) and [Modular Type Classes]([http://www.mpi-sws.org/~dreyer/papers/mtc/main-long.pdf), we propose a system for ad-hoc polymorphism in OCaml based on using modules as type-directed implicit parameters. You can try out an [interactive REPL](http://andrewray.github.io/iocamljs/modimp_show.html) of a prototype implementation online.

Our [modular implicits prototype](https://github.com/ocamllabs/ocaml-modular-implicits) was initially developed between Jan 2014 - Feb 2015, with more work taking place now in early 2017.

----

{% include news.html name="implicits" %}
