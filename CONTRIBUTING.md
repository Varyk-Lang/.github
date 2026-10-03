# Contributing to Varyk

Varyk is experimental and pre-1.0, and the design is still moving. The most
useful contributions right now are:

- trying the [examples](https://github.com/Varyk-Lang/varyk/tree/main/examples)
  and reporting what breaks or confuses you;
- comments on the design and on the
  [open questions](https://github.com/Varyk-Lang/varyk/blob/main/docs/open-questions.md),
  in [Discussions](https://github.com/Varyk-Lang/varyk/discussions);
- small, focused fixes.

Before starting a large change, open an issue so we can agree on the approach.
A change to the language surface starts in Discussions, not as a pull
request.

This guide applies to every repository in the Varyk-Lang organization that
has no `CONTRIBUTING.md` of its own. Where a repository has one, that file
applies instead.

## Pull requests

Varyk has one maintainer, so reviews are best effort and a pull request may
wait a while; a reminder after two weeks is welcome.

- Keep each pull request to one change.
- Run the checks the repository's CI runs before opening it; they are in
  `.github/workflows/`.
- Start the pull request title with a conventional prefix such as `feat:`,
  `fix:`, or `docs:`, and keep `<` and `>` out of it. In a repository that
  makes releases, the release notes are made from these titles.

## License

Unless you explicitly state otherwise, any contribution intentionally
submitted for inclusion in the work by you, as defined in the Apache-2.0
license, shall be dual licensed under MIT or Apache-2.0, without any
additional terms or conditions.

## Trademark

The name "Varyk" is covered by the project's
[trademark policy](https://github.com/Varyk-Lang/varyk/blob/main/TRADEMARKS.md).
Forks are welcome under a different name.

## Conduct

Everyone taking part follows the [code of conduct](CODE_OF_CONDUCT.md).
Security issues go to security@varyk.com, not to public issues; see
[SECURITY.md](SECURITY.md).
