# CHF thesis template

Starting point for an economics thesis or seminar talk at the Centre for Household Finance.
On GitHub click **Use this template → Create a new repository** to get your own copy, clone
that with GitHub Desktop, open the folder in VS Code, and start from `thesis.qmd`.

| File | What it is |
|---|---|
| `thesis.qmd` | Thesis skeleton: abstract, chapters with an equation and a citation, references, appendix. Renders to PDF. |
| `slides.qmd` | Beamer slide deck with one table and one figure. |
| `check.qmd` | Setup check for R, LaTeX, math, and citations. Render this first. |
| `check-python.qmd` | Setup check for Python and Jupyter. |
| `_quarto.yml` | Shared settings (bibliography, PDF layout). |
| `references.bib` | Your bibliography. Written by Zotero (Better BibTeX auto-export), never by hand. |

## Rendering

Open a `.qmd` file in VS Code and click **Preview** (top right). The first PDF may take a few
minutes while LaTeX fetches packages; later ones take seconds.

## References

Zotero is the only place references live. Add papers with the browser connector. Then, once
per project, connect Zotero to this folder's `references.bib`:

1. In Zotero, right-click **My Library** (or the collection for this thesis) → **Export Library…**
   (or **Export Collection…**).
2. Format: **Better BibTeX**. Tick **Keep updated**. Click OK.
3. Save the file as `references.bib` in this folder, replacing the one that is there.

From then on Zotero rewrites `references.bib` whenever the library changes. In a `.qmd` file,
type `@` and VS Code offers the keys from that file. Never edit `references.bib` by hand; if a
reference is wrong, fix it in Zotero. (Zotero → Settings → Better BibTeX → Automatic export
lists the exports it is keeping updated.)

The repo ships with a one-entry `references.bib` so that `check.qmd` renders before you have
done this.

## Citation style

The default is Chicago author-date. To switch, download a style file from
<https://www.zotero.org/styles> into this folder and add `csl: apa.csl` (or whichever) to
`_quarto.yml`.

## Before submitting

`thesis.qmd` is deliberately plain. Title page, declaration, and Faculty formatting rules are
handled at hand-in time.
