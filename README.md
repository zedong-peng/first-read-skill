# first-read-skill

A Claude Code skill for revising a research paper so that a careful first-time reader understands every sentence.

It was distilled from the way a senior researcher marks up a paper draft: where they highlight, and why. The skill holds the pattern, not the draft. Every example in it is invented.

The reader it describes stops at these things:

- a word used before it means anything,
- a verb that names no action,
- several mechanisms packed into one sentence,
- a sentence that defends instead of states,
- a paragraph that starts in the middle,
- a number the reader cannot place,
- arithmetic where the problem should be.

## Install

```sh
git clone https://github.com/zedong-peng/first-read-skill
ln -s "$PWD/first-read-skill/first-read" ~/.claude/skills/first-read
```

Then ask Claude Code to revise a draft with the `first-read` skill.
