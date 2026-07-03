# Review mode

Mark up prose for what to cut — a diff, a passage, a whole document, or a folder.
One line per finding: location, what, replacement. No rewrite — the deliverable is
the findings list. The draft's best outcome is getting shorter.

Scope scales with what you're handed:

- **Diff or passage** — the seven line tags, each finding in place.
- **Whole document or folder** — add the three structural tags a line scan can't
  see, rank findings biggest cut first, and close on a one-line structural verdict
  (the single highest-value change).

## Format

`L<n>: <tag> <what>. <replacement>.` — or `<file>:L<n>: ...` across files.

Line tags:

- `cut:` throat-clearing, meta-commentary, redundancy. Replacement: nothing.
- `merge:` two sentences carrying one idea, or a point already made elsewhere. Combine.
- `order:` buried point, old-after-new, lead not first. Move it to the front.
- `verb:` nominalization or weak verb. Name the strong verb.
- `show:` adjective or bare assertion where a number or evidence belongs. Name the number.
- `hedge:` hedge stack or reflexive CYA hedge (audience-conditional). Give the calibrated claim.
- `plain:` jargon the reader won't recognize and doesn't need. Give the plain word.
- `term:` a clause spelling out what one term of art names in a word, for a reader who shares the vocabulary. Name it — the mirror of `plain:`.
- `unbacked:` a claim or promised capability the document never delivers — a method named with no path, a hook with no follow-through, a feature with one mention and no milestone. Replacement: nothing, or back it.
- `scaffold:` a heading, framing, or defined term built up for a single payoff. Collapse it into the point it wraps.

`plain:` and `term:` are one rule split by audience, not two that disagree: name the
term of art when the reader owns the vocabulary, spell it out when they don't. The
audience picks the direction — never fire both on the same reader.

Structural tags — document- or folder-wide, what a line scan can't see:

- `struct:` a section that says nothing, or duplicates another. Cut or merge it.
- `bury:` the document's point — thesis, recommendation, key result — never surfaces, or surfaces too late. Move it to the front.
- `echo:` the same point made in three places. Keep the strongest, cut the rest.

## Examples

❌ "This opening paragraph feels a little long and might bury your main point — consider whether the reader gets to your contribution soon enough."

✅ `L1-4: order: contribution lands in sentence 5. Open on it.`

✅ `L7: cut: "It is worth noting that". Nothing replaces it.`

✅ `L12: show: "substantially improved". State the fold-change.`

✅ `L18: verb: "performed an analysis of". "analyzed".`

✅ `L23: hedge: "may potentially suggest". "suggests" — this is a results claim, not a limitation.`

## Hunt, document-wide

Sections that restate the abstract, paragraphs with no topic sentence, a thesis
that never appears, the same claim repeated across sections, throat-clearing
openings, hedge stacks, adjectives standing in for numbers, jargon that isn't a
term of art, capabilities promised but never built, claims with no support or
follow-through anywhere in the document, content that re-derives what a companion
document already establishes (reference it instead).

## Scoring

End with `net: -<N> words possible.` Over a whole document, rank findings biggest
cut first and add the one-line structural verdict. Nothing to cut: `Tight already.
Ship.`

## Boundaries

Scope: clarity, concision, and — document-wide — structure. Fact-checking, the
correctness of the underlying claims, and citation accuracy are out of scope —
route them to a subject-matter review. Never flag load-bearing structure (required
headings, normative keywords, acceptance criteria) or a load-bearing hedge for
deletion. Lists findings, applies nothing. "stop bluepencil-review" / "normal
mode": revert to verbose review style.
