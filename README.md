# Aleph Garden vocabularies

Published RDF vocabularies for [Aleph Garden](https://aleph.garden), a personal
semantic-web platform: your data as RDF in a store you own, queried
federatively, rendered through Fresnel-style lenses.

Terms are minted under `https://w3id.org/aleph/` and never under an
application's own domain, so an implementation may move and an identity may
not. This repository is the current serving location behind those permanent
identifiers, not the identifiers themselves — always cite the `w3id.org` form.

## Vocabularies

### Garden

Places concepts in a walkable world, connects them, routes through them, and
schedules their review. RDFS carries the taxonomy, SHACL carries the
conditions; there is deliberately no OWL, because open-world semantics
describes rather than constrains.

| Cite this | Served from |
|---|---|
| `https://w3id.org/aleph/garden#` | [`garden.ttl`](garden.ttl) |
| `https://w3id.org/aleph/garden/shapes` | [`garden-shapes.ttl`](garden-shapes.ttl) |

The shapes are the write contract rather than documentation: a store that
validates against them will reject a malformed write, and clients are expected
to treat their own checks as advisory.

## Status

The vocabulary is in use but has not been declared stable. Terms may still be
added, and the `w3id.org` redirects are `302` until they are.
