---
authors: [gemmag, avsm, kc]
title: "Maintaining the OCaml Compiler"
layout: page
---

{% mermaid %}
graph TD;
Platform("OCaml Platform")
click Platform "/platform/index.html" "Platform"
Compiler
click Compiler "/platform/compiler.html" "Compiler"
Platform --> Compiler
Compiler --> Maintenance
click Maintenance "/platform/compiler-maintenance.html" "Maintenance"
style Maintenance stroke:#000000,stroke-width:2px;
Maintenance --> CompilerPerformance
CompilerPerformance["Performance"]
Maintenance --> Portability
Maintenance --> Stdlib
Stdlib("Standard Library")
Maintenance --> Security
{% endmermaid %}
