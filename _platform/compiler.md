---
authors: [gemmag, avsm, kc]
title: "The OCaml Compiler"
layout: page
---

{% mermaid %}
graph TD;
Platform("OCaml Platform")
Platform --> Compiler
click Platform "/platform/index.html" "OCaml Platform"
style Compiler stroke:#000000,stroke-width:2px;
Compiler --> Maintenance
click Maintenance "/platform/compiler-maintenance.html" "Maintenance"
Compiler --> Features
Features["New Features"]
click Features "/platform/compiler-features.html" "Features"
Compiler --> CompilerTesting
CompilerTesting["Testing"]
click CompilerTesting "/platform/compiler-testing.html" "Compiler Testing"
{% endmermaid %}

The OCaml compiler has been under active development for over twenty years. We work on both maintaining the codebase, as well as adding new language and runtime features that are useful for using OCaml in large-scale codebases and on the latest hardware.

TODO

* **Maintaining** the large OCaml codebase is an important part of ensuring the long-term health of the language.
* **New Features** are selected by the needs of the Caml Consortium and our own experiences with large open-source scale codebases (e.g. MirageOS).

**Getting involved**

Maintenance -- Find a GitHub PR! Compiler Hacking sessions. Junior Jobs.

New Features -- contributing guide in OCaml, intern projects.
