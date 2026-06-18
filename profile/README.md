# 🚀 Aspect Starters

Ready-to-build [Bazel](https://bazel.build) starter projects, wired up with the
[Aspect CLI](https://docs.aspect.build/cli) and Aspect Workflows. Pick a
language, click **Use this template**, and start shipping — no Bazel
boilerplate, no toolchain yak-shaving.

## Two ways to start

**1. Use a template repo (this org)**

Each repo below is a GitHub *template repository*. Click the green **Use this
template** button (or **Fork**), or just:

```sh
git clone https://github.com/aspect-starters/<language>
```

**2. Scaffold with the Aspect CLI**

Already have the [Aspect CLI](https://docs.aspect.build/cli/install)? Generate a
project — choose a preset interactively, or pass one:

```sh
aspect init my-project --preset go
```

`aspect init` renders the same templates these repos are built from. No external
tools required.

## Starters

| Repo | Stack | Status |
| --- | --- | --- |
| [minimal](https://github.com/aspect-starters/minimal) | An empty, correctly-configured Bazel workspace | [![CI](https://github.com/aspect-starters/minimal/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/aspect-starters/minimal/actions/workflows/ci.yaml?query=branch%3Amain) |
| [go](https://github.com/aspect-starters/go) | Go | [![CI](https://github.com/aspect-starters/go/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/aspect-starters/go/actions/workflows/ci.yaml?query=branch%3Amain) |
| [py](https://github.com/aspect-starters/py) | Python | [![CI](https://github.com/aspect-starters/py/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/aspect-starters/py/actions/workflows/ci.yaml?query=branch%3Amain) |
| [js](https://github.com/aspect-starters/js) | JavaScript & TypeScript | [![CI](https://github.com/aspect-starters/js/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/aspect-starters/js/actions/workflows/ci.yaml?query=branch%3Amain) |
| [java](https://github.com/aspect-starters/java) | Java | [![CI](https://github.com/aspect-starters/java/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/aspect-starters/java/actions/workflows/ci.yaml?query=branch%3Amain) |
| [kotlin](https://github.com/aspect-starters/kotlin) | Kotlin | [![CI](https://github.com/aspect-starters/kotlin/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/aspect-starters/kotlin/actions/workflows/ci.yaml?query=branch%3Amain) |
| [scala](https://github.com/aspect-starters/scala) | Scala | [![CI](https://github.com/aspect-starters/scala/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/aspect-starters/scala/actions/workflows/ci.yaml?query=branch%3Amain) |
| [cpp](https://github.com/aspect-starters/cpp) | C & C++ | [![CI](https://github.com/aspect-starters/cpp/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/aspect-starters/cpp/actions/workflows/ci.yaml?query=branch%3Amain) |
| [rust](https://github.com/aspect-starters/rust) | Rust | [![CI](https://github.com/aspect-starters/rust/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/aspect-starters/rust/actions/workflows/ci.yaml?query=branch%3Amain) |
| [ruby](https://github.com/aspect-starters/ruby) | Ruby | [![CI](https://github.com/aspect-starters/ruby/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/aspect-starters/ruby/actions/workflows/ci.yaml?query=branch%3Amain) |
| [shell](https://github.com/aspect-starters/shell) | Bash / shell | [![CI](https://github.com/aspect-starters/shell/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/aspect-starters/shell/actions/workflows/ci.yaml?query=branch%3Amain) |
| [kitchen-sink](https://github.com/aspect-starters/kitchen-sink) | Everything — all languages + OCI, protobuf, release stamping, codegen | [![CI](https://github.com/aspect-starters/kitchen-sink/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/aspect-starters/kitchen-sink/actions/workflows/ci.yaml?query=branch%3Amain) |

## What every starter gives you

- 🧱 **Latest Bazel** (bzlmod) with curated flags via [`bazelrc-preset.bzl`](https://github.com/bazel-contrib/bazelrc-preset.bzl)
- 🧰 **Hermetic dev environment** via [`bazel_env.bzl`](https://github.com/buildbuddy-io/bazel_env.bzl) + [`rules_multitool`](https://github.com/theoremlp/rules_multitool)
- 🎨 **Formatting & linting** built in with [`rules_lint`](https://github.com/aspect-build/rules_lint), plus pre-commit hooks
- 📦 **Native package-manager integration** for the language (pip/uv, pnpm, go.mod, Cargo, Maven, Bundler, …)
- ⚙️ **Working GitHub Actions CI** that runs `aspect build`/`test`/`lint`/`format` on ephemeral runners — green out of the box
- 🐳 **OCI containers** via [`rules_oci`](https://github.com/bazel-contrib/rules_oci) (where applicable)
- 📌 A **pinned Aspect CLI version** (`.aspect/version.axl`) so your whole team and CI use the same tooling

## Building a polyglot monorepo?

Start from [**kitchen-sink**](https://github.com/aspect-starters/kitchen-sink) —
every language and feature wired together — or run `aspect init --preset
kitchen-sink`.

## Contributing

These repos are **generated artifacts**. The source of truth is
[**aspect-build/aspect-workflows-template**](https://github.com/aspect-build/aspect-workflows-template):
a single shared renderer produces both `aspect init` output and these starter
repos, and CI republishes them on every release. File issues and PRs there.

---

Built with ❤️ by [Aspect](https://aspect.build) — making Bazel Just Work™️.
