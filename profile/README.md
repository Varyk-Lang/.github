## Varyk

Varyk exists to make Rust available to everyone.

Rust is one of the safest and fastest languages there is, and one of the
hardest to learn. Its guarantees belong in every program, but its complexity
keeps most people out. Varyk keeps what makes Rust strong: memory safety
without a garbage collector, native speed, and the Rust ecosystem. It removes
the complexity that stands between people and those benefits, whether they
come from another language, are writing their first program, or are an AI
agent writing code.

Varyk compiles to Rust, the way TypeScript compiles to JavaScript. The Rust
compiler checks everything Varyk generates, so the guarantees are Rust's own.

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

Varyk is pre-0.1. Everything may change.

Created by [Vlad Mickevic](https://github.com/vlamic).

[varyk.com](https://varyk.com) · hello@varyk.com
