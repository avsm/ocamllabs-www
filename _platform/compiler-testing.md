---
authors: [gemmag, avsm, kc]
title: "Testing the OCaml Compiler"
layout: page
---

{% mermaid %}
graph TD;
Platform("OCaml Platform")
click Platform "/platform/index.html" "Platform"
Compiler
click Compiler "/platform/compiler.html" "Compiler"
Platform --> Compiler
Compiler --> CompilerTesting
style CompilerTesting stroke:#000000,stroke-width:2px;
CompilerTesting["Testing"]
CompilerTesting --> OCamlCI
OCamlCI["Continuous Integration"]
CompilerTesting ---> OCamlFuzz
OCamlFuzz["Fuzzing"]
{% endmermaid %}

The OCaml compiler has been under active development for over twenty years, and the codebase is complex after such a long period of sustained development.  TODO more.
