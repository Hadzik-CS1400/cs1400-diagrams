# cs1400-diagrams

Publicly hosted steppers and viewers for **CS 1400: Fundamentals of
Programming** at Weber State University.

**https://hadzik-cs1400.github.io/cs1400-diagrams/**

Each page is a single self-contained HTML file with no external references —
no CDN, no fonts, no analytics — so it works offline and on a locked-down
network once loaded.

| Page | Module | Source in the course repo |
|---|---|---|
| `demos/dictionaries.html` | 9 — Dictionaries | `module9-dictionaries/assignments/ct11-dictionary-basics/images/stepper.html` |
| `demos/files-exceptions.html` | 10 — File I/O & Exceptions | `module10-file-io-exceptions/assignments/ct12-file-io/images/stepper.html` |
| `demos/block-builder-week10.html` | 10 — Block Builder Week 10 | `block-builder-template/docs/week10_data.html` |
| `demos/plays-files.html` | Final Project — playtesting | `module-final-project/assignments/final-project/images/stepper.html` |
| `demos/random-and-seeds.html` | Block Builder — playtesting | `block-builder-template/docs/` |

The table was one row long for a while and the index page linked two of the
five files, so three of them were published and unreachable. If you add a
page, add it in **both** places.

## Steppers and viewers are not the same thing

Most of these walk a running program, one line per press, drawing what the
interpreter is actually doing beside the code.

`block-builder-week10.html` does not, and says so at the top. It is a
**refactor** — the code mostly stays where it is and the shape of the data
underneath it changes — so there is no line to walk. It puts the same program
before and after, one step per task, and names what the old shape could not
do. Nothing in it executes.

## This is a copy, not the source

The file of record lives in the course repository and ships in the student's
own starter repo. **Nothing links these copies back**, so they do not update
themselves — re-copy and push whenever one changes.

## What is safe to host here, and what is not

Nothing here is a solution to graded work *that is still open*. Students have
a byte-identical copy in their own repo, so hosting exposes nothing they do
not already hold.

That claim has a timing condition, and it is the only rule this repo really
has:

> **A page that shows a week's answer code must not be published before that
> week's deadline has passed.**

`block-builder-week10.html` is the case that makes it concrete. Its left-hand
column is sixty-four lines of **Week 9's answer**, and Week 9 is due at 08:30
on the Wednesday that answer is published. Publishing this page even a few
hours early would hand out that answer while submissions were still open —
which is exactly what the matched `due_at` / `lock_at` on every Block Builder
assignment exists to prevent. So it went up *after* the class repo did, not
before.
