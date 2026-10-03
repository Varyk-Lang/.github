## Varyk

Build backend services simply. Ship Rust binaries.

Varyk is a small language for APIs, workers, and microservices. It removes
Rust's ownership ceremony and keeps Rust's safety, speed, ecosystem, and
deployment model: you write Go-like application code, the compiler turns it
into readable Rust, rustc checks it, and you ship one native binary.

- No garbage collector, and no runtime beyond Rust's own.
- No lifetime annotations, no `&` or `&mut` to choose at a call site, and
  one string type.
- Cargo and crates.io underneath: a Varyk package is a Cargo package.
- Drop into Rust whenever you need it, in a `.rs` file beside your Varyk,
  in the same build.

```sh
cargo install varyk
```

The [compiler repository](https://github.com/Varyk-Lang/varyk) has the
[getting-started steps](https://github.com/Varyk-Lang/varyk#try-it) and the
[examples](https://github.com/Varyk-Lang/varyk/tree/main/examples).

Varyk exists so that ordinary backend services can be written simply and
shipped as safe Rust. It compiles to Rust the way TypeScript compiles to
JavaScript, though it is not a superset of Rust, and the Rust compiler
checks everything Varyk generates, so the guarantees are Rust's own.

```varyk
struct User {
    name: string,
}

fn rename(mut user: User) {
    user.name = "Bob";
}

fn print_user(user: User) {
    println!("{}", user.name);
}

fn main() {
    let mut user = User {
        name: "Alice",
    };

    print_user(user);
    rename(user);
    print_user(user);
}
```

It prints `Alice`, then `Bob`. Nothing in it says how a value is passed:
the compiler works that out, and rustc checks the result.

Varyk is experimental and pre-1.0: anything may change, and a breaking
change bumps the minor version. HTTP and databases, as packages, are next on
the [roadmap](https://github.com/Varyk-Lang/varyk/blob/main/docs/roadmap.md).
Questions and ideas are welcome in
[Discussions](https://github.com/Varyk-Lang/varyk/discussions).

Created by [Vlad Mickevic](https://github.com/vlamic).

[varyk.com](https://varyk.com) · hello@varyk.com
