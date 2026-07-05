# Review mode

Mark up prose for what to cut — a diff, a passage, a whole document, or a folder.
One line per finding: location, what, replacement. No rewrite — the deliverable is
the findings list. The draft's best outcome is getting shorter.

Scope scales with what you're handed:

- **Diff or passage** — each finding in place, tagged.
- **Whole document or folder** — the same tags, now firing at section and document
  scale too (a buried thesis, a claim echoed across sections, an over-scoped
  section); rank findings biggest cut first, and close on a one-line structural
  verdict (the single highest-value change).

## Format

`L<n>: <tag> <what>. <replacement>.` — or `<file>:L<n>: ...` across files. The span
carries the scale: a line, a range, or the whole document. Every tag is recursive —
it fires the same whether the defect is one sentence or one section; the line range
you cite says which.

Tags:

- `cut:` delete, no replacement — throat-clearing, meta-commentary, a framing built for a single payoff, a section that says nothing.
- `dupe:` said more than once — two sentences carrying one idea, a point already made, the same claim across sections. Combine if adjacent; keep the strongest and cut the rest if scattered. Load-bearing repetition is not a dupe: a deliberate bookend, a topic sentence and its elaboration, a plain-language gloss calibrating a technical claim, or units read independently and out of order (a figure caption and its body) all earn the repeat. Test: cut the second instance — does the reader lose orientation, emphasis, or audience access? If yes, keep it; flag only the echo that adds nothing.
- `order:` the point isn't at the front — buried in a subordinate clause, old-before-new, or a thesis/recommendation that never surfaces or surfaces too late. Move it to the front.
- `unbacked:` a promise with no path — a capability, hook, or whole section named with no method, milestone, or test. Back it or cut it. (Pass 2 works the cases.)
- `verb:` nominalization or weak verb. Name the strong verb.
- `show:` adjective or bare assertion where a number or evidence belongs. Name the number.
- `hedge:` hedge stack or reflexive CYA hedge (audience-conditional). Give the calibrated claim.
- `term:` jargon miscalibrated to the audience — the plain word when the reader doesn't own the vocabulary, the field's precise term when they do. One direction per reader; never fire both ways on the same reader.

## Examples

❌ "This opening paragraph feels a little long and might bury your main point — consider whether the reader gets to your contribution soon enough."

✅ `L1-4: order: contribution lands in sentence 5. Open on it.`

✅ `L7: cut: "It is worth noting that". Nothing replaces it.`

✅ `L12: show: "substantially improved". State the fold-change.`

✅ `L18: verb: "performed an analysis of". "analyzed".`

✅ `L23: hedge: "may potentially suggest". "suggests" — this is a results claim, not a limitation.`

✅ `L26: unbacked: "the toolkit will also generalize to streaming workloads" — one mention, no method or milestone. Cut or give it a path.`

✅ `L31,L52: dupe: the same limitation stated twice, sections apart. Keep the sharper one at L31, cut L52.`

✅ `L40-44: unbacked: the section names five deliverables in five sentences, none with an owner or date — over-scoped as a unit. Keep the one that's scoped; cut the rest.`

## Hunt, document-wide

Two passes, both required. Concision is one axis; delivery is the other. A
sentence can be tight, clear, and still a finding — because it promises what the
document never builds. Pass 1 catches words the reader shouldn't spend; Pass 2
catches claims the document doesn't earn.

**Pass 1 — reader effort (concision).** Sections that restate the abstract,
paragraphs with no topic sentence, a thesis that never appears (`order:`),
throat-clearing openings, hedge stacks, adjectives standing in for numbers,
jargon that isn't a term of art, the same claim repeated across sections
(`dupe:`) — matched on the claim's gist, not its wording: three differently
phrased sentences that all promise "the theory meets data" are one refrain, cut
to one. Cut too any content that re-derives what a companion document already
establishes — reference it instead.

**Pass 2 — earned claims (delivery).** Go claim by claim, paragraph by paragraph,
to the end, and for each ask both *where is the path?* — the method, the
milestone, the testable prediction — and *have I read this idea already?* A yes to
the second is a `dupe:` — unless the repeat is load-bearing (see the `dupe:` tag) —
however small or far apart: a claim restated as its own metaphor a sentence later
counts; a peroration that deliberately returns to the opening thesis for emphasis
does not. Flag with `unbacked:`:

- a capability named once with no method, milestone, or test — **even if the sentence is tight and clear**. Concision does not exempt it.
- a whole section that lists more ambitions than it can support, one sentence each, none with a path. Cite the section range; the unit is over-scoped, not any single line. Cut to the ones with tools in hand.
- a hook with no follow-through ("bears on disease," "opens the door to") — cut the hook or deliver on it.

The defect is the missing path, not the ambition. "I will do X" is a finding; "I
will do X via method Y, reaching milestone Z" is not. (Principle 4: aim = question
+ approach + expected outcome.) Never flag a claim the author supports elsewhere or
explicitly marks as an aim with a path.

## Scoring

End with `net: -<N> words possible.` Over a whole document, rank findings biggest
cut first and add the one-line structural verdict. A cut licensed by `unbacked:`
counts the same as a concision cut — an unearned claim is words the reader spends
on a promise the document breaks. Clean on both passes: `Nothing to cut, nothing unbacked. Leave it as written.`

## Boundaries

Scope: clarity, concision, and — document-wide — structure and earned claims.
Internal delivery is in scope; external truth is not. Whether the document backs
its own claim is yours to flag (`unbacked:`). Whether the claim is true in the world,
the citations, the underlying science: out of scope — route to a subject-matter
review. Never flag load-bearing structure (required headings, normative keywords,
acceptance criteria) or a load-bearing hedge for deletion. Lists findings, applies
nothing. "stop bluepencil-review" / "normal mode": revert to verbose review style.
