---
authors: [gemmag, avsm, kc]
title: "Developing new features for the OCaml Compiler"
layout: page
---

{% mermaid %}
graph TD;
Platform("OCaml Platform")
click Platform "/platform/index.html" "Platform"
Compiler
click Compiler "/platform/compiler.html" "Compiler"
Platform --> Compiler
Compiler --> Features
Features["New Features"]
click Features "/platform/compiler-features.html" "Features"
style Features stroke:#000000,stroke-width:2px;
Features --> Multicore
click Multicore "/platform/multicore.html" "Multicore"
Features --> Implicits
click Implicits "/platform/implicits.html" "Implicits"
Features --> Macros
click Macros "/platform/macros.html" "Macros"
Features --> Namespacing
click Namespacing "/platform/namespaces-module-aliases.html" "Namespacing"
{% endmermaid %}

We have worked on numerous new features for the OCaml language.  Our current
projects are:

* **[Multicore OCaml]({% link _platform/multicore.md %}):** adding shared memory parallelism to OCaml.
* **[Modular Implicits]({% link _platform/implicits.md %}):** supporting ad-hoc polymorphism in the language.
* **[Macros]({% link _platform/macros.md %}):** a language extension for compile-time metaprogramming.
* **[Namespacing]({% link _platform/namespaces-module-aliases.md %}):** a means for grouping the components of a library together.

## Getting involved

**TODO** good intern projects, check on GitHub, contact feature person, look at compiler hacking sessions.
