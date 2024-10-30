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

# Miscellaneous Tools & Crates
* [Rust Playground](https://play.rust-lang.org/)
  * very full-featured
     * tools incl. `Clippy`, `rustfmt`, `Miri` and macro expansion (nightly only)
     * supported output formats incl. asm, wasm and Rust's various IRs
     * only really lacks a REPL :-)
* [cargo-expand](https://crates.io/crates/cargo-expand)
  * outputs the exansions of the current crate's `macro_rules!`s and `#derive`s
* [pest](https://pest.rs) parser
  * [awesome pest](https://github.com/pest-parser/awesome-pest)
* [Rayon](https://crates.io/crates/rayon)
  * [work-stealing](https://github.com/rayon-rs/rayon/blob/main/FAQ.md#how-does-rayon-balance-work-between-threads) data-parallelism library in the vein of [Cilk](https://en.wikipedia.org/wiki/Cilk) / [OpenCilk](https://www.opencilk.org)
    * cf. the [Rust + Cilk](https://dspace.mit.edu/handle/1721.1/156790) extension (work in progress)
* [SQLx](https://crates.io/crates/sqlx)
  * async SQL toolkit w/ compile-time checked queries
  * [ecosystem](https://github.com/launchbadge/sqlx/wiki/Ecosystem) incl. ORMs, notably [SeaORM](https://crates.io/crates/sea-orm)
* [hyper](https://crates.io/crates/hyper)
  * HTTP library leveraged by [tokio](https://crates.io/crates/tokio) and, inter alia:
    * [warp](https://crates.io/crates/warp) - web server framework
    * [reqwest](https://crates.io/crates/reqwest) - HTTP client lib
    * [axum](https://crates.io/crates/axum) - web app framework
* [Crossbeam](https://crates.io/crates/crossbeam)
  * various tools for concurrent programming, including MPMC channels
  * the project's wiki incl. a list of (non-Rust specific) resources on concurrent programming & related topics
 
# Testing
* [QuickCheck](https://crates.io/crates/quickcheck)
  * property-based testing
* [proptest](https://crates.io/crates/proptest)
  * property-based testing
  * more actively maintained than quickcheck, inspired by Python's [Hypothesis](https://hypothesis.works)
    * [differences between quickcheck and proptest, from the README](https://github.com/proptest-rs/proptest?tab=readme-ov-file#differences-between-quickcheck-and-proptest)
  * [proptest book](https://proptest-rs.github.io/proptest/)
* [cargo-fuzz](https://crates.io/crates/cargo-fuzz)
  * CLI front-end for [libFuzzer](https://llvm.org/docs/LibFuzzer.html)
* [Mockall](https://crates.io/crates/mockall)
  * mocking lib - the [automock](https://docs.rs/mockall/latest/mockall/attr.automock.html) macro is particularly convenient
* [Criterion](https://crates.io/crates/criterion)
  * microbenchmarking lib inspired by [its Haskell namesake](https://hackage.haskell.org/package/criterion)
   
# Embedded Rust
* [Embedded Rust doc](https://docs.rust-embedded.org)
* [Embassy](https://embassy.dev/)
  * async Rust for embedded

# Operating Systems Development in Rust
* Incomplete/not necessarily up-to-date lists of OSes written (for the most part) in Rust:
  * [Awesome Rust/Operating Systems](https://github.com/rust-unofficial/awesome-rust?tab=readme-ov-file#operating-systems)
  * [Comparison of OSes written in Rust](https://github.com/flosse/rust-os-comparison)
* [Rust OSDev](https://rust-osdev.com)
  * publishes monthly updates dedicated to OS development in Rust
* [CharlotteOS](https://www.charlotte-os.org)
* [Hermit for Rust](https://github.com/hermit-os/hermit-rs)
  * unikernel
* [Rust for Linux](https://rust-for-linux.com)
* [Redox OS](https://www.redox-os.org)
  * [Redox OS book](https://doc.redox-os.org/book/)

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
* [Asynchronous Programming in Rust](https://rust-lang.github.io/async-book/) - AKA the Async Book
* [Work-stealing & Share-nothing](https://without.boats/blog/thread-per-core/)
* [Async: What is blocking?](https://ryhl.io/blog/async-what-is-blocking/)
* [Actors with Tokio](https://ryhl.io/blog/actors-with-tokio/)
* [Tree-Structured Concurrency](https://blog.yoshuawuyts.com/tree-structured-concurrency/)
* [Why Async Rust](https://blog.yoshuawuyts.com/why-async-rust/)
  * goes into a lot of detail about async Rust's internals, their motivations and ramifications
* Cancellations:
  * [Async Cancellation](https://blog.yoshuawuyts.com/async-cancellation-1/)
  * [Async Cancellation II: Time and Signals](https://blog.yoshuawuyts.com/async-cancellation-2/)
* Popular Async runtimes:
  * [Tokio](https://crates.io/crates/tokio) and [the Tokio stack](https://tokio.rs) are the de-facto standards
  * [async-std](https://crates.io/crates/async-std) aims to offer "an async version of std"
    * [async-std book](https://book.async.rs)
  * [smol](https://crates.io/crates/smol) aims to be small and fast
  * [Datadog's Glommio](https://crates.io/crates/glommio) leverages io_uring (so is Linux-only)

# Rust and WebAssembly
* [rustwasm Website](https://rustwasm.github.io) and [GitHub repo](https://github.com/rustwasm)
  * [rustwasm doc](https://rustwasm.github.io/docs.html)
    * the [Rust and WebAssembly book](https://rustwasm.github.io/docs/book/) provides a natural starting point w/ both [tutorial](https://rustwasm.github.io/docs/book/game-of-life/introduction.html) and [reference](https://rustwasm.github.io/docs/book/reference/index.html) sections
    * [wasm-bindgen guide](https://rustwasm.github.io/docs/wasm-bindgen/)
    * [wasm-pack book](https://rustwasm.github.io/docs/wasm-pack/)
   
# TLS Libs
* [Rustls](https://crates.io/crates/rustls) - TLS lib written in Rust
  * [audit report (from 2020)](https://github.com/rustls/rustls/tree/main/audit)
  * [related libs](https://github.com/rustls), notably:
    * [hyper-rustls](https://crates.io/crates/hyper-rustls)
    * [tokio-rustls](https://crates.io/crates/tokio-rustls)
* [native-tls](https://crates.io/crates/native-tls/0.2.12)
  * abstracts over OS-specific crates that provide bindings for said OSes' native TLS libs
  * powers [tokio-native-tls](https://crates.io/crates/tokio-native-tls)
* Comparisons between Rustls and native-tls:
  * [A brief guide to choosing TLS crates (reddit/r/rust)](https://www.reddit.com/r/rust/comments/1454654/a_brief_guide_to_choosing_tls_crates/)
  * [`Prefer `rustls` over `native_tls`?` (URLO thread)](https://users.rust-lang.org/t/prefer-rustls-over-native-tls/90137)
