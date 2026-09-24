# Security policy

## Reporting a vulnerability

Email security@varyk.com. Do not open a public issue.

Include what you found, how to reproduce it, and the version or commit you
tested. Varyk is maintained by one person, so replies are best effort: you
will hear back as soon as possible, and if you have heard nothing after two
weeks, please send a reminder. Once a fix is ready, it is released and the
report is credited unless you ask otherwise.

## Scope

Reports are welcome for anything in the Varyk-Lang organization, in
particular:

- the compiler producing Rust that behaves differently from the Varyk source,
  or that bypasses a check Varyk promises to make;
- the compiler reading or writing files outside the project and its build
  directory;
- the website and install instructions pointing somewhere they should not.

A bug in rustc or in a Rust crate that Varyk uses belongs with that project.
If you are not sure, write to us anyway.

## Supported versions

Varyk is pre-0.1. Only the latest release and the `main` branch receive fixes.
