# Contributing to Varyk

Varyk is experimental and pre-0.1, and the design is still moving. The most
useful contributions right now are:

- trying the examples and reporting what breaks or confuses you;
- comments on the design and on the open questions, in the issues;
- small, focused fixes.

Before starting a large change, open an issue so we can agree on the approach.
A change to the language surface starts as a design discussion, not a pull
request.

## Pull requests

Varyk has one maintainer, so reviews are best effort and a pull request may
wait a while; a reminder after two weeks is welcome.

- Keep each pull request to one change.
- Run `cargo fmt`, `cargo clippy --workspace --all-targets -- -D warnings`,
  and `cargo test --workspace` before opening it. CI runs the same checks.
- A change to the language surface updates `docs/language.md` in the same
  pull request.

## License

Unless you explicitly state otherwise, any contribution intentionally
submitted for inclusion in the work by you, as defined in the Apache-2.0
license, shall be dual licensed under MIT or Apache-2.0, without any
additional terms or conditions.

## Trademark

The name "Varyk" is covered by the project's trademark policy, `TRADEMARKS.md`
in the main repository. Forks are welcome under a different name.

## Conduct

Everyone taking part follows the [code of conduct](CODE_OF_CONDUCT.md).
Security issues go to security@varyk.com, not to public issues; see
[SECURITY.md](SECURITY.md).
