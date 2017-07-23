---
authors: [gemmag, avsm, kc]
title: "The OCaml Platform"
layout: page
---

{% mermaid %}
graph TD;
Platform("OCaml Platform")
click Platform "/platform/index.html" "Platform"
style Platform stroke:#000000,stroke-width:2px;
Compiler
click Compiler "/platform/compiler.html" "Compiler"
Platform --> Compiler
Platform --> Toolchain
click Toolchain "/platform/toolchain.html" "Toolchain"
{% endmermaid %}

The focus of the OCaml Platform is to improve the use of OCaml for large scale codebases, such as those found in [industrial settings](https://ocaml.org/consortium/) or large open source projects such as [Ocsigen](http://ocsigen.io) or [MirageOS](https://mirage.io).  This involves improving the core compiler to add features and maintain the codebase, as well the toolchain around documentation, packaging, build and test infrastructure.  There is currently no formal release of the Platform, and the first one is currently [being worked on](/platform/bob.html).

**Getting involved:** The Platform effort is a collaborative one, involving many developers that work on different areas.  We welcome contributors who wish to get help with the first release, and so each of the areas being worked on below has more details.

**Release Cycle:** TODO


**The [OCaml compiler]({% link _platform/compiler.md %}):** This has been under active development for over twenty years. We work on both maintaining the codebase, as well as adding new language and runtime features that are useful for using OCaml in large-scale codebases and on the latest hardware.

**The OCaml toolchain:** We have also been systematically working on a set of tools that address how to code, build test and package an OCaml project.  In the first few years of development, this effort has resulted in improvements to the core language, as well as the development of brand new tools. Our efforts are now focussed on building a single developer-facing tool that unifies the tooling into one single binary that provides a single point of integration for the workflow.

### Build, Package and Release

* [Merlin IDE integration]({% link _doc/merlin.md %})
* [Opam package management]({% link _doc/opam.md %})
* [OCaml Documentation]({% link _doc/documentation.md %})
* [Packaging workflow]({% link _doc/packaging.md %})
* [Digital signing with Conex]({% link _doc/conex.md %})
* [Bulk builds]({% link _doc/bulk-builds.md %})
* [Windows support]({% link _doc/windows.md %})

### Test

* [Continuous Integration and Testing]({% link _doc/testing.md %})

### Popular libraries

* [Ctypes]({% link _doc/ctypes.md %})

----

{% include news.html name="platform" %}
