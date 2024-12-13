# Abstract Machines vs Concrete Outcomes
* [Uninitialised memory & UB](https://www.ralfj.de/blog/2019/07/14/uninit.html)
  * cf. David Chisnall's [C Is Not a Low-level Language](https://queue.acm.org/detail.cfm?id=3212479) (which the piece above refers to)
  * pointers & pitfalls:
    * [pointer semantics](https://www.ralfj.de/blog/2018/07/24/pointers-and-bytes.html)
    * [aliasing, alias analysis and pointer provenance](https://faultlore.com/blah/fix-rust-pointers/#background)

# C
* [ISO Standards](https://www.iso-9899.info/wiki/The_Standard)
* [cppreference.com](https://en.cppreference.com/w/)
  * references for C and C++ - the languages as well as their standard libraries
* C's ABI(s):
  * [C Isn't A Programming Language Anymore](https://faultlore.com/blah/c-isnt-a-language/)
    * [More on the C ABI](https://thephd.dev/to-save-c-we-must-save-abi-fixing-c-function-abi)
* [From C to LLVM IR to x86-64 asm](https://ocw.mit.edu/courses/6-172-performance-engineering-of-software-systems-fall-2018/resources/lecture-5-c-to-assembly/)
  * great intro lecture & slides
* Modeling C's Semantics:
  * [The C standard formalized in Coq](https://robbertkrebbers.nl/thesis.html) (C11)
  * [C semantics](https://github.com/kframework/c-semantics) (C17) for the [K Framework](https://github.com/runtimeverification/k)
  * [Cerberus](https://www.cl.cam.ac.uk/~pes20/cerberus/) (C11)
* C runtime:
  * [crt0 entry on Wikipedia](https://en.wikipedia.org/wiki/Crt0)
  * [Program Initialization (OSDev.org)](https://wiki.osdev.org/Creating_a_C_Library#Program_Initialization)
* libc:
  * [C standard library (Wikipedia overview)](https://en.wikipedia.org/wiki/C_standard_library)
  * [glibc manuals](https://sourceware.org/glibc/manual/)
    * as of this writing 2.22 -> 2.40 are available in multiple formats (including HTML and PDF)

# CHERI
* [CHERI's page on the Uni of Cambridge's site](https://www.cl.cam.ac.uk/research/security/ctsrd/cheri/)
  * part of the [CTSRD project](https://www.cl.cam.ac.uk/research/security/ctsrd/)
* [CTSRD-CHERI repo](https://github.com/CTSRD-CHERI)
* [CheriBSD](https://www.cheribsd.org)
  * [CheriBSD 24.05 getting started doc](https://ctsrd-cheri.github.io/cheribsd-getting-started/) for the [Arm Morello eval board](https://www.arm.com/architecture/cpu/morello)
