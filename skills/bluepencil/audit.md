# Audit mode

Review mode, document-wide. Scan a whole document — or a folder of documents —
instead of a diff. Rank findings biggest cut first. One-shot report; applies
nothing.

## Tags

The line tags from [`review.md`](review.md): `cut`, `merge`, `order`, `verb`,
`show`, `hedge`, `plain`. Plus **structural** tags a line scan can't see:

- `struct:` a section that says nothing, or duplicates another. Cut or merge it.
- `bury:` the document's point — thesis, recommendation, key result — never surfaces, or surfaces too late. Move it to the front.
- `echo:` the same point made in three places. Keep the strongest, cut the rest.

## Hunt

Sections that restate the abstract, paragraphs with no topic sentence, a thesis
that never appears, the same claim repeated across sections, throat-clearing
openings, hedge stacks, adjectives standing in for numbers, jargon that isn't a
term of art.

## Output

One line per finding, ranked biggest cut first:
`<tag> <what to cut>. <replacement>. [path:L<n>]`

End with `net: -<N> words possible.` plus a one-line structural verdict (the
single highest-value change). Nothing to cut: `Tight already. Ship.`

## Boundaries

Scope: clarity, concision, and structure only. Correctness of the claims and
citation accuracy are out of scope. Never flag load-bearing structure (required
headings, normative keywords, acceptance criteria) or a load-bearing hedge for
deletion. Lists findings, applies nothing. One-shot. "stop bluepencil-audit" /
"normal mode" to revert.
