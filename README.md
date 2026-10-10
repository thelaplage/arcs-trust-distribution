# ARCS Trust Distribution — v0.1.0

This repository is a **neutral public transport surface** for byte-exact copies
of governed ARCS/DAGR verification material. It is not itself a trust authority.

Version tag: `trust-material-v0.1.0`

## Transport boundary

- Governance / trust membership remains governed elsewhere.
- Trust-bundle custody remains in `thelaplage/dagr-ops`.
- Key↔principal binding custody remains in `thelaplage/dagr-runtime`.
- Publication does not establish truth, standing, admission, or EXIT-O closure.
- Use the immutable version tag, not `main` or any moving branch, for verification.

The two governed JSON files below are byte-exact copies of their pinned custody
sources. They must not be reformatted or reserialized in this distribution.

### Trust bundle

File: `srs-trust-bundle.dagr-ops.production.v0.2.6b043c9c8428.json`

- source: `thelaplage/dagr-ops@86250b31cd04e49e82531cfe70ef074a19ab4580`
- source blob: `6205f900d36c15808371cf6f7f04438ae5cadfc7`
- byte length: `1158`
- transport SHA-256: `f77527c1ae4bf08a559debe82b54d99785c55a3a78ed4f5b7a50f37785753420`
- logical bundle digest:
  `sha256:6b043c9c84288ac03bf4830040958d4f69bcc0fa0e122de9e3e9d8eb5f80b264`

### Key↔principal binding

File: `dagr-institutional-key-principal-binding.v0.1.semantic-origin.2026-09.7e572dac0c58.json`

- source: `thelaplage/dagr-runtime@47792714b1b0ca2d9787ff4adbc73aed138a86d8`
- source blob: `c25ecf38535524435d9f2bb91eb242a81ae44894`
- byte length: `941`
- transport SHA-256: `c740517c9b09c97dec18a946d7a5a558a95fe160b1a85ad18754e09d73bcfa67`
- logical binding digest:
  `sha256:7e572dac0c5850fee4adbb30a3db3bc2a6d1cd2a9624168c97b708433f1e727d`

## Immutable tag-pinned locators

`https://raw.githubusercontent.com/thelaplage/arcs-trust-distribution/trust-material-v0.1.0/srs-trust-bundle.dagr-ops.production.v0.2.6b043c9c8428.json`

`https://raw.githubusercontent.com/thelaplage/arcs-trust-distribution/trust-material-v0.1.0/dagr-institutional-key-principal-binding.v0.1.semantic-origin.2026-09.7e572dac0c58.json`

`SHA256SUMS` intentionally inventories only these two published governed payloads.
The prepublication candidate manifest used to prepare this publication is not a
public distribution artifact because it described these locators as
`prospective_unserved` before the publication act.

Verifier pin for the current acceptance line (a commit that resolves in the
public `thelaplage/arcs-verify` repository):
`arcs-verify@9e6daefca6e77306691fd288880448194bd28f75`.

Install: `pip install "arcs-verify @ git+https://github.com/thelaplage/arcs-verify@9e6daefca6e77306691fd288880448194bd28f75"`.

The earlier pin `arcs-verify@e30d8d634897fbb1ea1c8cd58ae4c4b13e6ff2aa` named a
private-development commit. The public `arcs-verify` repository is a fresh
snapshot that does not contain that history, so that commit did not resolve
publicly (HTTP 422 from the GitHub commits API, observed 2026-10-09). The earlier
text remains in the immutable `trust-material-v0.1.0`, `trust-material-v0.1.1` and
`counterpedia-mcp-live0-trust-v0.1.0` tags, which are not rewritten. The verifier
bytes at the public pin are not asserted to be identical to the earlier pin.
A commit in a snapshot repository stays resolvable only while that history is
not replaced; this is not a tag or release.

Retrieval failure is distinct from retrieved-but-invalid. Public retrieval and
byte identity establish **trust-material independence**, not production trust
authority and not EXIT-O completion.
