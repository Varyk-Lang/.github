# Security policy

## Reporting a vulnerability

Email security@varyk.com, or use **Report a vulnerability** in the
repository's Security tab. Do not open a public issue.

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
- a package such as varyk-sql placing a value into the text of a query
  instead of beside it, or passing the message of an internal failure on
  to a client;
- the website and install instructions pointing somewhere they should not.

A bug in rustc or in a Rust crate that Varyk uses belongs with that project.
If you are not sure, write to us anyway.

## Supported versions

Varyk is pre-1.0. Only the latest release and the `main` branch receive fixes.
