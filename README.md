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

**Experimental — do not build on this yet.** The garden vocabulary is a working
draft: terms may be renamed or removed outright, not merely added, and the
model is still moving.

The `w3id.org` identifiers are permanent; the documents behind them are not.
Redirects stay `302` until the vocabulary is declared stable.

## Licence

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Each vocabulary also
carries its licence and creator as `dcterms:` triples, so the terms travel with
the document rather than with this repository.

Referencing the terms — writing `garden:PlaceCard` into your own graph — is not
redistribution and needs no attribution. Attribution applies when you share the
vocabulary itself: copying a document, deriving another vocabulary from it, or
publishing it onward. In that case name the title, the author, a link to the
source, and the licence:

> "Aleph Garden vocabulary" by Christopher Mühl,
> <https://w3id.org/aleph/garden>, licensed under
> [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

State it too if you changed anything.
