# Aleph Garden vocabularies

Published RDF vocabularies for [Aleph Garden](https://aleph.garden), a personal
semantic-web platform: your data as RDF in a store you own, queried
federatively, rendered through Fresnel-style lenses.

Terms are minted under `https://w3id.org/aleph/ns/` and never under an
application's own domain, so an implementation may move and an identity may
not. This repository is the current serving location behind those permanent
identifiers, not the identifiers themselves — always cite the `w3id.org` form.

Vocabularies are named for their subject, not for the application that first
needed one: the food vocabulary is shared by everything that keeps stock, cooks
from it or shops for it, and naming it after any one of those would have made
the other two look like guests in it.

## Vocabularies

### Lens

Which view is offered for a subgraph, and what draws it. A lens describes a way
of looking at several resources rather than a single one — that is the line
against SHACL, which says what may be written about one node. Where a view is a
form or a card over one node, a shape already answers it and no lens is needed.

| Cite this | Served from |
|---|---|
| `https://w3id.org/aleph/ns/lens#` | [`lens.ttl`](lens.ttl) |

### Food

How much of what. A recipe line, a lot in a cupboard and a wish on a list are
the same statement — a substance and an amount — and only that sameness makes
"does the stock cover the recipe" answerable. An amount carries its shape
outright, because a reader has to see at a glance whether arithmetic is allowed:
measured amounts may be converted, counted ones lack a dimension, hand measures
are words rather than units, and an unspecified amount is a state rather than a
missing value.

| Cite this | Served from |
|---|---|
| `https://w3id.org/aleph/ns/food#` | [`food.ttl`](food.ttl) |
| `https://w3id.org/aleph/ns/food/shapes` | [`food-shapes.ttl`](food-shapes.ttl) |

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

**Experimental — do not build on this yet.** These are working drafts: terms
may be renamed or removed outright, not merely added, and the models are still
moving.

The garden vocabulary predates the `/ns/` layout and still sits at
`https://w3id.org/aleph/garden#`. It will move rather than stay the exception,
but not before it is worth renaming once instead of twice.

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

> "Aleph Garden food vocabulary" by Christopher Mühl,
> <https://w3id.org/aleph/ns/food>, licensed under
> [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

State it too if you changed anything.
