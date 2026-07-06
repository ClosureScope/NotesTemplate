# NotesTemplate

Starter template for a Typst course-notes repository. Click **"Use this
template"** on GitHub to create a new course repo, then:

1. **Edit `course.toml`** — set `name_en`, `name_zh`, `code` for your course.
2. **Rename / write `notebook.typ`** — this is your actual notes file.
   (You can have multiple `.typ` files; all except `template.typ` get compiled.)
3. **Push.** CI (via [`NotesCI`](https://github.com/ClosureScope/NotesCI)) will
   compile the PDF, publish it to Releases, and regenerate this README.

## What's in here

| File | Purpose |
|------|---------|
| `course.toml` | Course metadata — the only file you routinely edit |
| `notebook.typ` | Your notes (starter stub) |
| `template.typ` | Styling template, imported by the notes |
| `.github/workflows/auto_release.yml` | 6-line stub that calls the reusable workflow in `NotesCI` |

## Requirements

The build logic lives in the public repo `ClosureScope/NotesCI`. This README
(and the release name) are generated from `course.toml`, so you never edit them
by hand.
