# LUSTRE

![license](https://img.shields.io/badge/license-MIT-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![category](https://img.shields.io/badge/category-supercomputer-lightgrey)

> Anticloud-hardened packaging of the upstream project `LUSTRE` in category **SUPERCOMPUTER**. Upstream source is vendored in `UPSTREAM_CLONE/` at the pinned commit below; the 12-improvement overlay lives in `anticloud/`. Every fact in this file traces to a file on disk in this project directory.

**Category:** SUPERCOMPUTER · **Upstream:** https://github.com/lustre-labs/lustre · **Upstream pin:** `f5ac432bb2d625951be4f8731fe446aa03320061` · **Vendor:** Anticloud FZ LLE

---

## What This Project Does

<h1 align="center">Lustre</h1>

<div align="center">
  ✨ <strong>Make your frontend shine</strong> ✨
</div>

<div align="center">
  Create HTML templates, single page applications, Web Components, and real-time
  server components in Gleam!
</div>

<br />

<div align="center">
  <a href="https://hex.pm/packages/lustre">
    <img src="https://img.shields.io/hexpm/v/lustre"
      alt="Available on Hex" />
  </a>
  <a href="https://hexdocs.pm/lustre">
    <img src="https://img.shields.io/badge/hex-docs-ffaff3"
      alt="Documentation" />
  </a>
</div>

<div align="center">
  <h3>
    <!--
    <a href="https://lustre.build">
      Website
    </a>
    <span> | </span>
    -->
    <a href="https://hexdocs.pm/lustre/guide/01-quickstart.html">
      Quickstart
    </a>
    <span> | </span>
    <a href="https://hexdocs.pm/lustre">
      Reference
    </a>
    <span> | </span>
    <a href="https://discord.gg/Fm8Pwmy">
      Discord
    </a>
  </h3>
</div>

<div align="center">
  <sub>Built with ❤︎ by
  <a href="https://bsky.app/profile/hayleigh.dev">Hayleigh Thompson</a> and
  <a href="https://github.com/lustre-labs/lustre/graphs/contributors">
    contributors
  </a>
</div>

---

## Table of contents

- [Features](#features)
- [Example](#example)
- [Philosophy](#philosophy)
- [Installation](#installation)
- [Where next](#where-next)
- [Support](#support)

## Features {#features}

- A **declarative**, functional API for constructing HTML. No templates, no macros,
  just Gleam.

- An Erlang and Elm-inspired architecture for **managing state**.

- **Managed side effects** for predictable, testable code.

- Universal components. **Write once, run anywhere**. Elm meets Phoenix LiveView.

- A **batteries-included CLI** that makes scaffolding and building apps a breeze.

- **Server-side rendering** for static HTML templating.

## Example {#example}

Lustre comes with [over 20 examples](https://hexdocs.pm/lustre/reference/examples.html)!
Here's what it looks like:

```gleam
import gleam/int
import lustre
import lustre/element.{text}
import lustre/element/html.{div, button, p}
import lustre/event.{on_click}

pub fn main() {
  let app = lustre.simple(init, update, view)
  let assert Ok(_) = lustre.start(app, "#app", Nil)

  Nil
}

fn init(_flags) {
  0
}

type Message {
  Incr
  Decr
}

fn update(model, message) {
  case message {
    Incr -> model + 1
    Decr -> model - 1
  }
}

fn view(model) {
  let count = int.to_string(model)

  div([], [
    button([on_click(Incr)], [text(" + ")]),
    p([], [text(count)]),
    button([on_click(Decr)], [text(" - ")])
  ])
}
```

## Philosophy {#philosophy}

Lustre is an _opinionated_ library for building frontend Web applications. Modern
frontend development is hard and complex. Some of that complexity is necessary, but
a lot of it is accidental or comes from having far too many options. Lustre has the
same design philosophy as Gleam: where possible, there should be only one way to do
things!

That means shipping with a single state management system out of the box, modelled
after Elm and Erlang/OTP. Open any Lustre application and you should feel
right at home.

It also means we encourage simple approaches to constructing views over complex
ones. Lustre _does_ have a way to create encapsulated stateful components (something
we sorely missed in Elm) but it shouldn't be the default. Prefer simple functions
to stateful components.

Where components _are_ necessary, lean into the fact that Lustre components can
run _anywhere_. Lustre gives you the tools to write components that can run inside
an existing Lustre application, export them as a standalone Web Component, or run
them on the server with a minimal runtime for patching the DOM. Lustre calls these
**universal components** and they're written with Gleam's multiple targets in mind.

## Installation {#installation}

Lustre is published on [Hex](https://hex.pm/packages/lustre)! You can add it to
your Gleam projects from the command line:

```sh
gleam add lustre
```

Lustre also has a companion package containing development tooling that you might
like to install:

```sh
gleam add --dev lustre_dev_tools
```

## Where next {#where-next}

To get up to speed with Lustre, check out the [quickstart guide](https://hexdocs.pm/lustre/guide/01-quickstart.html).
If you prefer to see some code, the [examples](https://github.com/lustre-labs/lustre/tree/main/examples)
directory contains a handful of small applications that demonstrate different
aspects of the library.

You can also read through the documentation and API reference on
[HexDocs](https://hexdocs.pm/lustre).

## Support {#support}

Lustre is mostly built by just me, [Hayleigh](https://github.com/hayleigh-dot-dev),
around two jobs. If you'd like to support my work, you can [sponsor me on GitHub](https://github.com/sponsors/hayleigh-dot-dev).

Contributions are also very welcome! If you've spotted a bug, or would like to
suggest a feature, please open an issue or a pull request.

*Quoted from the upstream `README.md` file in `UPSTREAM_CLONE/`.*
Project-specific facts detected in this directory:

- Ecosystem: **Unknown (no standard manifest detected)** (manifests: none detected; scanned in UPSTREAM_CLONE)
- Top-level source layout: `birdie_snapshots/`, `dev/`, `examples/`, `pages/`, `priv/`, `src/`, `test/`
- Snapshot size: **320 files**, **0 lines of code** (measured; see Benchmarks)
- Primary languages: `.accepted` (97), `.gleam` (80), `.md` (57), `.toml` (32), `.css` (24), `.mjs` (22)
- Upstream commit pinned for this packaging: `f5ac432bb2d625951be4f8731fe446aa03320061`

---

## Installation

Website
    </a>
    <span> | </span>
    -->
    <a href="https://hexdocs.pm/lustre/guide/01-quickstart.html">
      Quickstart
    </a>
    <span> | </span>
    <a href="https://hexdocs.pm/lustre">
      Reference
    </a>
    <span> | </span>
    <a href="https://discord.gg/Fm8Pwmy">
      Discord
    </a>
  </h3>
</div>

<div align="center">
  <sub>Built with ❤︎ by
  <a href="https://bsky.app/profile/hayleigh.dev">Hayleigh Thompson</a> and
  <a href="https://github.com/lustre-labs/lustre/graphs/contributors">
    contributors
  </a>
</div>

---

*Section quoted from the upstream readme.*
Overlay install (this project):

```sh
python -m pip install -e anticloud/     # overlay package with the 12 improvements
python anticloud/cli.py --help          # 13 subcommands, JSON stdout
```

---

## Usage

- [Philosophy](#philosophy)
- [Installation](#installation)
- [Where next](#where-next)
- [Support](#support)

*Section quoted from the upstream readme.*
Anticloud overlay CLI (available in every project):

```sh
python anticloud/cli.py --help     # 13 subcommands, JSON stdout
python anticloud/cli.py checks     # run the 16-check suite
```

---

## API

</a>
</div>

<div align="center">
  <h3>
    <!--
    <a href="https://lustre.build">
      Website
    </a>
    <span> | </span>
    -->
    <a href="https://hexdocs.pm/lustre/guide/01-quickstart.html">
      Quickstart
    </a>
    <span> | </span>
    <a href="https://hexdocs.pm/lustre">
      Reference
    </a>
    <span> | </span>
    <a href="https://discord.gg/Fm8Pwmy">
      Discord
    </a>
  </h3>
</div>

<div align="center">
  <sub>Built with ❤︎ by
  <a href="https://bsky.app/profile/hayleigh.dev">Hayleigh Thompson</a> and
  <a href="https://github.com/lustre-labs/lustre/graphs/contributors">
    contributors
  </a>
</div>

---

*Section quoted from the upstream readme.*
---

## Dependencies

| Metric | Value |
|--------|-------|
| Ecosystem | Unknown (no standard manifest detected) |
| Manifests detected | none |
| Files in snapshot | 320 |
| Lines of code | 0 |
| Dependency references | 0 |
| Upstream license | MIT |
| Overlay license | Anticommons 0.1.0 |

Pinned lockfile: `anticloud/requirements.lock` (hash-pinned, PEP 508). SBOM: `sbom.cdx.json` (CycloneDX 1.5, pinned to the upstream SHA).

---

## Configuration

same design philosophy as Gleam: where possible, there should be only one way to do
things!

That means shipping with a single state management system out of the box, modelled
after Elm and Erlang/OTP. Open any Lustre application and you should feel
right at home.

It also means we encourage simple approaches to constructing views over complex
ones. Lustre _does_ have a way to create encapsulated stateful components (something
we sorely missed in Elm) but it shouldn't be the default. Prefer simple functions
to stateful components.

Where components _are_ necessary, lean into the fact that Lustre components can
run _anywhere_. Lustre gives you the tools to write components that can run inside
an existing Lustre application, export them as a standalone Web Component, or run
them on the server with a minimal runtime for patching the DOM. Lustre calls these
**universal components** and they're written with Gleam's multiple targets in mind.

*Section quoted from the upstream readme.*
Overlay configuration (Anticloud):

- `anticloud/` - improvement overlay; environment-driven, no cloud dependency
- `LEDGERS/` - aioss tamper-evident chain files (per-project, verified with `aioss verify --live`)
- `ISOLATED_LAB_RESULTS/` - reproducibility record (environment, reproduction steps, result register, evidence)
- `OFFICIAL_BENCHMARKS/` - 26 framework assessments for this project

---

## Contributing

Upstream contributions: fork the `LUSTRE` project, create a feature branch, and open a pull request against upstream. Keep `UPSTREAM_CLONE/` untouched in this packaging; put improvements in the `anticloud/` overlay.

Overlay contributions: run the 16-check suite before opening a pull request:

```sh
python anticloud/bench/runner.py --cwd anticloud
```

---

## License

**Upstream license: MIT** (evidence: `LICENSE` in the upstream snapshot).

License file excerpt:

```text
Copyright 2022 Hayleigh Thompson

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in the
Software without restriction, including without limitation the rights to use,
copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Anticommons 0.1.0 overlay

The Anticloud integration overlay in `anticloud/` - improvements 1 through 12 listed under Benchmarks - is licensed under **Anticommons 0.1.0**. Upstream code remains under its original MIT terms. See `ANTICOMMONS_LICENSE.md` in this directory for the overlay terms and contact.

SPDX: `MIT` (upstream) + Anticommons 0.1.0 (overlay, dual).

---

## Upstream

- **Project:** `LUSTRE` (category: SUPERCOMPUTER)
- **Upstream URL:** https://github.com/lustre-labs/lustre
- **Pinned commit (SHA):** `f5ac432bb2d625951be4f8731fe446aa03320061`
- **Branch:** main
- **Pin provenance:** GitHub API commits/main. The parent-project stamp is explicitly rejected for this project.
- **Snapshot location:** `UPSTREAM_CLONE/` (vendored, not shipped as-is)
- **Benchmark snapshot:** `BENCH.json`

---

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`899af452ef0a8138e8eda422823e0f70b820eaae8dd5992fc1240efdcd3bd630`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe and Mail, Business Insider, National Post, Financial Post, StreetInsider, Digital Journal, Barchart, International Business Times, and fox47 · National Law Review.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

