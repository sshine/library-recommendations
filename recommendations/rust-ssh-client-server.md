# SSH client + server libraries in Rust

**Review made:** Jan 21, 2023

There are several Rust libraries that deal with the SSH 1 + 2 protocol.

Some are client-only libraries, others support both client and server.

Some wrap libssl2, others are pure Rust implementations.

At the time of writing, these stood:

- The [ssh](https://crates.io/crates/ssh) crate: 8k total downloads, updated 7 years ago.
- The [ssh2](https://crates.io/crates/ssh2) crate: 706k total downloads, release 1 year ago, git activity 3 weeks ago.
- The [thrussh](https://crates.io/crates/thrussh) crate: 103k total downloads, release 1 year ago, pijul activity Aug 2019.
- The [russh](https://crates.io/crates/russh) crate: 10k total downloads, release 2 weeks ago, git activity 1 week ago.
- The [ssh-rs](https://crates.io/crates/ssh-rs) crate: 2k total downloads, release 2 weeks ago, git activity 1 week ago.

Some evaluation:

- "ssh" is dead by all accounts. It was a libssh2 bindings library, client only.
- "ssh2" is the most mature bindings to libssh2, client only.
- "russh" is a fork of "thrussh" with several additions, client and server, under active development.
- "ssh-rs" is a similar project, client and server. Seems slightly less mature, but under active development.

## Assessment

### Jan 21, 2023

I'd definitely go with "russh" at this point.
