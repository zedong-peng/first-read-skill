---
name: first-read
description: Revise a research paper so that a careful first-time reader understands every sentence. Use when revising a paper draft after a senior reader marked it up, or before sending a draft to one.
---

The reader is a senior researcher in the field who has not seen this project. They read once, in order, with a highlighter. They do not look ahead for a definition and do not guess what a word means. Every highlight is a place where they stopped. Revise so that they never stop.

## What makes them stop

**A word used before it means anything.** A coined name, an abbreviation, a label taken from a figure, or a common word used in a private sense ("the baseline", "the fast path", "stage", "shard"), or the field's own jargon when the venue is broader than the subfield. Each term is defined once, in plain words, at its first use, and means the same thing everywhere after. If the paper has three names for one thing, keep one. Coin a name only for what the paper will refer to many times; everything else is described.

- Before: "We eliminate join stalls via plan-wide key realignment."
- After: "The two inputs of a join often arrive sorted on different keys, so the join waits for one input to finish and sorts it again. We sort that input on the other input's key when it is first written."

**A verb that names no action.** Coordinate, reconcile, select, leverage, address, handle, enable, account for. After such a sentence the reader cannot say what the system did. Write what is read, written, moved, compared or waited for, and by which component.

- Before: "The scheduler coordinates batch size with memory constraints."
- After: "The scheduler picks the largest batch whose intermediate results fit in memory."

**Several mechanisms in one sentence.** A sentence that lists three interacting things explains none of them. One sentence carries one step; the next sentence carries the next. A long noun phrase joined by "and" or "while preserving" is usually three sentences.

**A sentence that defends instead of states.** "Rather than measured…", "although X could…", "this does not guarantee…", "we note that…", "it should be mentioned…". The reader asked for none of it, and each one makes the result sound weaker than the table shows. Delete them. What the experiment measured, on what, and how, is stated once, plainly, in the setup; it is not repeated as an apology beside every number.

**A paragraph that starts in the middle.** A paragraph that opens with "Figure 4 shows…" or with its first example has not said why the reader is here. Open with one sentence that places it: what stage the system is at, and what goes wrong there. Then the figure and the examples.

**A number the reader cannot place.** "Took 41 ms, against 17 ms predicted and a 30 ms budget" makes the reader work out which comparison matters. Give the one comparison that carries the point (it missed the budget) and leave the rest to the table.

**Arithmetic where the problem should be.** The motivation says what goes wrong and what it costs, with one concrete example and its numbers. Derivations, index algebra and the full parameter space belong to the design section. If a paragraph in the motivation needs four symbols, keep the example and cut the algebra to one sentence.

## What to keep

- Names that appear in figures, and the names of the contributions. Changing them in the text alone breaks the match between figure and prose; change both or neither.
- Numbers. A rewrite for readability changes no value and no claim. If a sentence cannot be made plain without changing what it claims, the claim is the problem; raise it.
- Facts that change how a number is read. Removing a hedge is not the same as hiding a fact. When a deleted caveat carried one (a different input, a different machine, a projected rather than measured value), say the fact once as a plain statement of method, or list it for the authors to decide. Never let a reader conclude something the data does not show.

## How to work

1. Read the marked pages first and sort the marks into the kinds above. The unmarked pages have the same problems; the reader simply has not reached them.
2. List every term the paper coins or uses in a private sense. For each: keep and define once, replace with a description, or delete.
3. Rewrite paragraph by paragraph, one sentence per line, so that the authors can see each change. Do not reorder the argument unless asked.
4. Read the result as the reader would: in order, stopping at every word that has not been introduced.
5. Report what changed in a few lines, and list separately the deleted caveats that carried a fact.
