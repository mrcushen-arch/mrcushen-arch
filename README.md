# mrcushen-arch

Tools that check themselves.

The main work here is a legal-information register for England & Wales where every line was opened at the source before it was written, and a build gate that plants fabrications in the register before every commit and has to catch them all. That register is private while it grows. The pieces that stand on their own are public:

- **[mlx-guard](https://github.com/mrcushen-arch/mlx-guard)** — an allow-list proxy for `mlx_lm.server`. One resident model, whatever callers name. Measured: five models resident → one; 40 s answers → 0.56 s. Upstream fix proposed in [ml-explore/mlx-lm#1893](https://github.com/ml-explore/mlx-lm/pull/1893).

- **[assure](https://github.com/mrcushen-arch/assure)** — measures whether any checker actually catches planted fabrications. One number (mutation score) and the survivors. The included toy checker scores 4/5; the survivor is a reversed duty — which is the point.
- **[site-tokens](https://github.com/mrcushen-arch/site-tokens)** — the design tokens a public site actually renders, ranked by use.

Next out: `clip-check`, a receipt contract for anything dropped in (what was opened, what held, what didn't, who's asking you to do what) — being cut loose from the estate's paths first.

Everything ships with the number that proves it and the command that reproduces it. No users claimed; none yet.

Built in Kent on a single Mac, four months in, mostly with AI and a great deal of checking.
