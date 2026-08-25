# Aleph Garden vocabularies

[Aleph Garden](https://aleph.garden) is an attempt at keeping personal data as
RDF in a store you own, querying it across your own and other people's
endpoints, and drawing it through views you can swap out. These are the
vocabularies it publishes.

The shapes alongside them are a write contract rather than documentation: a
store that validates against them rejects a malformed write, and a client's own
checks are advisory.

## Vocabularies

### Lens

Which view is offered for a subgraph, and what draws it. A lens describes a way
of looking at several resources rather than a single one — that is the line
against SHACL, which says what may be written about one node.

| Cite this | Served from |
|---|---|
| `https://w3id.org/aleph/ns/lens#` | [`lens.ttl`](lens.ttl) |

### Food

**Playground.**

How much of what. A recipe line, a lot in a cupboard and a wish on a list are
the same statement — a substance and an amount — and only that sameness makes
"does the stock cover the recipe" answerable. An amount carries its shape
outright, so that a reader sees at a glance whether arithmetic is allowed here.

| Cite this | Served from |
|---|---|
| `https://w3id.org/aleph/ns/food#` | [`food.ttl`](food.ttl) |
| `https://w3id.org/aleph/ns/food/shapes` | [`food-shapes.ttl`](food-shapes.ttl) |

### Garden

**Playground.**

Places concepts in a walkable world, connects them, routes through them, and
schedules their review. RDFS carries the taxonomy, SHACL carries the
conditions; there is deliberately no OWL, because open-world semantics
describes rather than constrains.

| Cite this | Served from |
|---|---|
| `https://w3id.org/aleph/ns/garden#` | [`garden.ttl`](garden.ttl) |
| `https://w3id.org/aleph/ns/garden/shapes` | [`garden-shapes.ttl`](garden-shapes.ttl) |

## Status

**Experimental — do not build on this yet.** Terms may be renamed or removed
outright, not merely added. The `w3id.org` identifiers are permanent even so;
the documents behind them are not, and redirects stay `302` until a vocabulary
is declared stable.

## Licence

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Each vocabulary
carries its licence and creator as `dcterms:` triples, so the terms travel with
the document rather than with this repository.

Writing `garden:PlaceCard` into your own graph is use, not redistribution, and
needs no attribution. Attribution applies to sharing a vocabulary itself —
copying it, deriving another from it, publishing it onward:

> "Aleph Garden food vocabulary" by Christopher Mühl,
> <https://w3id.org/aleph/ns/food>, CC BY 4.0 — changed from the original.
