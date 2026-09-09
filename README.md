# Nicolas Dréno

Solution architect, France. I build API and AI gateway infrastructure in Rust, and platform architecture for enterprises.

CTO of [Barbacane](https://barbacane.dev/), consultant with Gluendo.

## Building

| Project | What it is |
| --- | --- |
| **[barbacane](https://github.com/barbacane-dev/barbacane)** | API and bidirectional AI gateway in Rust. OpenAPI and AsyncAPI specs are the only configuration, with no proprietary DSL: the spec is compiled into an artifact and enforced as a contract. WASM plugins, AGPL-3.0. |
| **[parapet](https://github.com/barbacane-dev/parapet)** | SecLang rule engine in pure Rust, compatible with the OWASP Core Rule Set. Apache-2.0. |
| **[typify](https://github.com/barbacane-dev/typify)** | Compiler from JSON Schema into idiomatic Rust types. Apache-2.0. |
| **[tofu-plan-comment](https://github.com/ndreno/tofu-plan-comment)** | Forgejo/GitHub Action that posts `tofu plan` output as a single, updated-in-place pull request comment. MIT. |

## How I work

I use LLM agents heavily, and I bound them on both sides. Intent lives outside the model, in versioned artifacts (specs, ADRs, LLDs, schemas as code), and blocking gates verify what has to be true (pre-commit hooks, CI, linters, coverage floors, supply chain checks). The agent gets a lot of freedom in between, and none at the edges.

On Barbacane that means 8 specs and 31 ADRs written before the code, 16 CI jobs on every pull request, `cargo deny` on a schedule, and keyless signing plus SBOM attestation on every image.

I write about this, and about platform architecture, on **[blog.gluendo.com](https://blog.gluendo.com)**.

## Recent open source contributions

- **[beerjson](https://github.com/beerjson/beerjson)**: migrated the format to JSON Schema 2020-12, fixed the doc and type generator, closed 9 of 13 `allOf` types to unknown keys, and made the npm package usable.
- **[warpgate](https://github.com/warp-tech/warpgate)** and **[terraform-provider-warpgate](https://github.com/warp-tech/terraform-provider-warpgate)**: global parameters from Warpgate 0.27, acceptance tests for the parameters resource.
- **[terraform-provider-netbox](https://github.com/e-breuninger/terraform-provider-netbox)**: description and comments on `netbox_device_type`.
- **[rke2-charts](https://github.com/rancher/rke2-charts)**: Cilium 1.20.0.

## Interests

Spec-driven systems, API and AI gateways, Kubernetes platform engineering, infrastructure as code, supply chain security. Rust, Go, OpenTofu, NetBox.

I also brew beer, which is the honest reason I contribute to BeerJSON.

## Elsewhere

- Blog: [blog.gluendo.com](https://blog.gluendo.com)
- Barbacane: [barbacane.dev](https://barbacane.dev/)
