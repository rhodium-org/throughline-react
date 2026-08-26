# throughline-react

The **Airbnb React/JSX Style Guide** expressed as a
[throughline](https://pypi.org/project/throughline/) **source** — a standalone,
grounded requirements graph that a consuming project composes with
[throughline-compose](https://github.com/rhodium-org/throughline-compose).

This repository holds no code. It is a directory of small YAML items with permanent
UIDs, validated by `tl check`. Consumers import it under a namespace and reference its
rules as `react:SR-0001`.

## A framework-style source

`throughline-react` is a **framework style** source: it governs how React components
are authored, orthogonal to the language source you compose alongside it. A TypeScript
React project would typically compose `throughline-typescript` (language) **and**
`throughline-react` (framework) at once.

## Status

<!-- tl:count type == 'user_requirement' -->
15
<!-- tl:end --> sections and
<!-- tl:count type == 'system_requirement' -->
36
<!-- tl:end --> style rules, published to [`docs/spec.md`](docs/spec.md):

- `INT-0001` — the root intent (why the guide exists), `normative: false`.
- Each major guide section as a `user_requirement` that `derives_from` the intent.
- Every individual rule as a `system_requirement` that `implements` its section,
  carrying the guide reference in `attrs.source_ref`.

The counts above are rendered from the live graph by the `tl:count` directive, so they
cannot drift.

## Editions — dated tags

The guide is a living document. A material revision is cut as a dated tag on this repo
(e.g. `v2026-08`); a consumer pins the ref it wants.

## Composing it

```toml
[[sources]]
namespace = "react"
url = "https://github.com/rhodium-org/throughline-react"
ref = "v2026-08"
```

Then reference a rule from your own items:

```yaml
links:
- target: react:SR-0001      # Airbnb React/JSX Style Guide: include only one component per file
  type: satisfies
```

`tl-compose check` resolves the reference; bare `tl check` fails fast and points you at
`tl-compose`.

## Local checks

```sh
pip install throughline
tl check --strict     # the graph must stay sound
tl docs --check       # docs/spec.md must match the graph
```

## Provenance

The Airbnb React/JSX Style Guide is © Airbnb, licensed MIT. See [NOTICE](NOTICE) and
https://airbnb.io/javascript/react/. This repository is Apache-2.0 for its structure
and tooling; the reproduced rule text remains Airbnb's.
