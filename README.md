# mrcushen-arch

Tools that check themselves.

The main work here is a legal-information register for England & Wales where every line was opened at the source before it was written, and a build gate that plants fabrications in the register before every commit and has to catch them all. That register is private while it grows. The pieces that stand on their own are public:

- **[mlx-guard](https://github.com/mrcushen-arch/mlx-guard)** — an allow-list proxy for `mlx_lm.server`. One resident model, whatever callers name. Measured: five models resident → one; 40 s answers → 0.56 s. Upstream fix proposed in [ml-explore/mlx-lm#1893](https://github.com/ml-explore/mlx-lm/pull/1893).

Coming out as they're cut loose from the estate: `assure` (measures whether any checker catches planted fabrications), `site-tokens` (computed-style design tokens from any public site), `clip-check` (a receipt contract for anything dropped in: what was opened, what held, what didn't, who's asking you to do what).

Everything ships with the number that proves it and the command that reproduces it. No users claimed; none yet.

Built in Kent on a single Mac, four months in, mostly with AI and a great deal of checking.
