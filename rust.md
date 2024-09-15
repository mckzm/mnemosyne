# General Learning Resources
* [Yet Another Rust Resource (YARR!)](https://yarr.fyi/introduction)
  * the best learning resource I know of for Rust beginners
    * [its objectives, and how to use it, are explained in a blog post by Nicole, its author](https://ntietz.com/blog/introducing-yet-another-rust-resource-or-yarr/)
* [The Rust Programming Language](https://doc.rust-lang.org/stable/book/) AKA the Rust Book
* [Brown University's version of the Rust Book](https://rust-book.cs.brown.edu)
  * spruced up with visualisations and a whole lot of interactive quizzes, in particular IRT ownership and UB
* [Learn Rust with Entirely Too Many Linked Lists](https://rust-unofficial.github.io/too-many-lists/index.html)
  * A great way to delve deeper into the language's semantics, and a very fun read :-)
* [Learning Rust](https://quinedot.github.io/rust-learning/) by QuineDot
  * particularly helpful/enlightening on borrows/lifetimes and `dyn Trait`
* [Rust for Rustaceans](https://rust-for-rustaceans.com)
* [std's doc](https://doc.rust-lang.org/stable/std/)
* [The Little Book of Rust Macros](https://veykril.github.io/tlborm/)

# Hands-On Learning Resources
* [Rust by Example](https://doc.rust-lang.org/stable/rust-by-example/) (browser/playground-based)
  * best read in tandem with [QuineDot's Notes](https://github.com/QuineDot/rbe-notes)
* [Rustlings](https://rustlings.cool) (local install)
* [100 Exercises To Learn Rust](https://rust-exercises.com/100-exercises/)
  * offers a gentle intro to systems programming concepts
  * longer, more life-like examples than Rustlings and RBE
  * covers [Tokio](https://tokio.rs)
* [Rust by Practice](https://practice.course.rs)
* [Exercism's Rust track](https://exercism.org/tracks/rust)
* [MacroKata](https://tfpk.github.io/macrokata/index.html)
  * `macro_rules!` only as of this writing
* [Procedural Macros Workshop](https://github.com/dtolnay/proc-macro-workshop)

# Rust & Functional Programming (FP)
* Many of Rust's FP-supporting features and idiosyncracies are nicely outlined in:
  * [Is Rust functional?](https://tech.fpcomplete.com/blog/2018/10/is-rust-functional/)
  * [Collect in Rust, traverse in Haskell and Scala](https://tech.fpcomplete.com/blog/collect-rust-traverse-haskell-scala/)
  * [Rust for Haskell Developers](https://serokell.io/blog/rust-for-haskellers)

# Type System
* [The Pain Of Real Linear Types in Rust](https://faultlore.com/blah/linear-rust/)
* [More on affine typing in Rust](https://without.boats/blog/ownership/)
* [Defaults Affect Inference in Rust: Expressions Instead Of Types](https://faultlore.com/blah/defaults-affect-inference/)

# Tools, Crates Etc.
* [Rust Playground](https://play.rust-lang.org/)
  * very full-featured
     * tools incl. `Clippy`, `rustfmt`, `Miri` and macro expansion (nightly only)
     * supported output formats incl. asm, wasm and Rust's various IRs
     * only really lacks a REPL :-)
* [cargo-expand](https://crates.io/crates/cargo-expand)
  * outputs the exansions of the current crate's `macro_rules!`s and `#derive`s
* [Criterion](https://crates.io/crates/criterion)
  * microbenchmarking lib inspired by [its Haskell namesake](https://hackage.haskell.org/package/criterion)
* [QuickCheck](https://crates.io/crates/quickcheck)
  * property-based testing
* [cargo-fuzz](https://crates.io/crates/cargo-fuzz)
  * CLI front-end for [libFuzzer](https://llvm.org/docs/LibFuzzer.html)
* [pest](https://pest.rs) parser
  * [awesome pest](https://github.com/pest-parser/awesome-pest)
   
# Embedded Rust
* [Embedded Rust doc](https://docs.rust-embedded.org)
* [Embassy](https://embassy.dev/)
  * async Rust for embedded

# Operating Systems in Rust
* [Awesome Rust/Operating Systems](https://github.com/rust-unofficial/awesome-rust?tab=readme-ov-file#operating-systems)
* [Comparison of OSes written in Rust](https://github.com/flosse/rust-os-comparison)

# Internals
* [The Rust Reference](https://doc.rust-lang.org/stable/reference/)
* [Raph Lieven's Container Cheat Sheet](https://docs.google.com/presentation/d/1q-c7UAyrUlM-eZyTo1pd8SZ0qwA_wYxmPZVOQkoDmH4/)
* [Rustonomicon](https://doc.rust-lang.org/stable/nomicon/)
* [The rustc Book](https://doc.rust-lang.org/rustc/index.html)
* [Rust Compiler Development Guide](https://rustc-dev-guide.rust-lang.org/getting-started.html)
* [DSTs Are Just Polymorphically Compiled Generics](https://faultlore.com/blah/dsts-are-polymorphic-generics/)
* [Rust Atomics and Locks](https://marabos.nl/atomics/)
* [AtomicUsize, Mutex, and interior mutability](https://leon.schuermann.io/blog/2024-08-07_rust-mutex-atomics-unsafecell_spooky-action-at-a-distance.html)

# Design & Perf
* [How to Code It](https://www.howtocodeit.com)
* [Modular Errors in Rust](https://sabrinajewson.org/blog/errors)
* [Effective Rust](https://www.lurklurk.org/effective-rust/title-page.html)
* [The Rust Performance Book](https://nnethercote.github.io/perf-book/introduction.html)
* [Nesting Allocators](https://blog.yoshuawuyts.com/nesting-allocators/)
* [Circular References](https://mckayla.blog/posts/circular-references.html)
  * safe & unsafe Rust compared w/ Go and Zig

# Async Rust
* [Asynchronous Programming in Rust](https://rust-lang.github.io/async-book/)
* [Async: What is blocking?](https://ryhl.io/blog/async-what-is-blocking/)
* [Actors with Tokio](https://ryhl.io/blog/actors-with-tokio/)
* [Tree-Structured Concurrency](https://blog.yoshuawuyts.com/tree-structured-concurrency/)
