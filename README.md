> **This repository has moved to [llorracc/DecentralizingRCK](https://github.com/llorracc/DecentralizingRCK).** This copy is archived and
> is no longer updated; the current handout, its notebook and its history are there.

# Decentralizing the Ramsey/Cass-Koopmans Model

A handout for JHU Econ 180.603 (Intertemporal Choice): an economy of households and firms trading in competitive
markets reaches the allocation of the Ramsey/Cass-Koopmans planner, under conditions that the handout states, and
it fails to when those conditions fail.

- **The source is the book's chapter,** [Decentralizing the Ramsey/Cass-Koopmans Model](https://intertemporal-choice.github.io/content/growth/decentralizingrck/)
  (`content/growth/DecentralizingRCK.md` in
  [intertemporal-choice.github.io](https://github.com/intertemporal-choice/intertemporal-choice.github.io)).
  Edits start there and are carried into `DecentralizingRCK.tex`.
- **Build:** `latexmk` (the `latexmkrc` points TeX at the vendored registry in `@resources/`, econ-ark-tools
  02e344d5, notation v14.1.0, read-only).
- **Check against the book:** `./check-book-sync.py` (the book's main on GitHub), or
  `./check-book-sync.py --book-git <clone> --ref <commit>` for an unpushed book commit. It compares the words,
  the notes (a `\marginFootnote` here is a margin note in the book), the links, the citations and the printed
  symbols, and checks rule D: every object written with its macro.
- `@local/DecentralizingRCK.sty` defines no notation. Since 17b6cc5 (registry v14.1.0) the registry has every object
  this handout writes, the rental rate `\kapRent`, productivity `\PtyLab`, the Hamiltonian `\Ham` and the costate
  `\vk` among them.
- `DecentralizingRCK.bib` holds the entries the handout cites, copied verbatim from texmf-local's `economics.bib`;
  the empty `system.bib` keeps the build to them.

Revived on 2026-11-17 from the 2021 handout (the first commit holds it as found, including `LaTeX/`).
