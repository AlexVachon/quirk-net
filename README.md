# net

Network entry point. Re-exports the high-level `Socket` struct and exposes the low-level POSIX-style socket primitives that `Socket` is built on. Most users want `from net.socket use { Socket }` for t

This package is also bundled with the Quirk compiler at
`<QUIRK_HOME>/packages/net/`, so `use net` works out of the box on a
fresh install. This repo is the canonical home — when you want a version
newer than the one your compiler shipped with, install it explicitly:

```bash
quirk pkg install net             # latest tag from this repo
quirk pkg install net@1.0.0       # pinned
```

The compiler-shipped registry maps the bare name `net` to this repo
(since v1.4.0), so no `quirk pkg registry add` is needed.

## Origin

Split from `quirk-compiler/packages/net/` in compiler v1.5.0 as part of
the stdlib-in-independent-repos rollout. Source history before that lives
in [AlexVachon/quirk](https://github.com/AlexVachon/quirk).

## License

MIT (see [`LICENSE`](LICENSE)).
