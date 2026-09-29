# 01 — Layered Imprint Constraint Analysis (LICA)

## Purpose

LICA is the custom method used in this package. It is not a new laboratory instrument. It is a decision procedure for combining heterogeneous Shroud observations so that a medieval-artist hypothesis, a generic-crucified-man hypothesis, and a Jesus-of-Nazareth hypothesis can be scored against the same constraint stack.

It exists because product-of-independents calculations (Barberis 1/200 billion; de Gail 1/225 billion) look precise and are not. They smuggle in independence and arbitrary priors. LICA replaces that with **layered vetoes** plus a conservative Bayesian sketch.

## Five layers

```
L1  Photochemical     What is the image, physically?
L2  Temporal          In what order did blood and image form?
L3  Forensic          What happened to the body?
L4  Geometric         How did cloth and body relate in space?
L5  Historical        Does the object have a pre-Lirey path, and does it match a named man?
```

A hypothesis is **eliminated** if it fails a hard constraint in L1–L3.  
A hypothesis is **weakened** if it fails a soft constraint in L4–L5.  
Identity with Jesus is an L5 inference that is only licensed after L1–L4 survive.

## Hard constraints (veto)

A viable image-formation or authorship hypothesis must simultaneously satisfy all of the following. Failure on any one is fatal.

1. **No applied pigment sufficient to form the body image.** X-ray fluorescence, microchemistry, UV, IR (STURP 1978; Schwalbe & Rogers 1982; Jumper et al. 1984).
2. **Color confined to the primary cell wall**, on the order of 0.2–0.6 µm, not a painted film.
3. **Photographic negativity** discovered by Secondo Pia (1898) and confirmed on every subsequent plate. Artists do not paint in negative as a default 14th-century technique.
4. **Distance encoding.** Image intensity maps to cloth-to-body distance (Jackson, Jumper & Ercoline 1984, *Applied Optics* 23:2244). VP-8 relief is anatomically coherent, not a bas-relief artifact alone.
5. **Blood before image.** No body-image chromophore under bloodstains. Blood soaked, clotted, and transferred first; image formed later around it.
6. **Blood chemistry positive** for heme / porphyrin / albumin (Heller & Adler 1980, 1981).
7. **Non-contact facial resolution.** Direct-contact-only mechanisms cannot produce the face’s spatial frequency content (STURP official summary).
8. **Scorch vs image distinction.** 1532 fire scorches fluoresce under UV; the body image does not (Miller / Pellicori UV photography).

## Soft constraints (weight, not veto)

9. Alternative dating cluster (vanillin absence, Fanti FTIR/Raman/mechanical, De Caro WAXS) compatible with 1st century under stated assumptions.
10. Gospel-level forensic specificity: cap of thorns, wrist not palm, side wound, no crurifragium, hasty burial, no decomposition image.
11. Sudarium of Oviedo congruence (documented by 1075).
12. Pre-1355 iconographic echoes (Pray Codex 1192–1195; Vignon / Mandylion chain).

## Scoring rules

Each constraint is tagged:

- `ESTABLISHED` — multi-lab or STURP-consensus physical observation
- `SUPPORTED` — peer-reviewed, limited replication
- `CONTESTED` — real expert disagreement
- `SPECULATIVE` — do not load-bear

Only `ESTABLISHED` items may veto.  
`SUPPORTED` items shift likelihood.  
`CONTESTED` items are shown both ways in `docs/07_objections.md`.  
`SPECULATIVE` items (Catalano overlays, coin-over-eyes, most pollen claims) have weight ≈ 0.

## What LICA is not

- Not a claim that ultraviolet radiation from a resurrection has been measured.
- Not a replacement for new sampling of the cloth.
- Not Barberis’ product of seven made-up fractions.
- Not a dismissal of the 1988 radiocarbon result; that result is an objection, documented, then excluded from the user-requested posterior.

## Decision output

After stacking:

- Medieval pigment-artist hypothesis: **eliminated** by L1 hard constraints.
- Medieval contact-transfer / bas-relief hypothesis: **severely weakened** by L1+L2+L4 (fails blood-before-image, UV fluorescence distinction, and simultaneous 3-D + superficiality + non-contact face). Moraes 2025 is treated as a live geometric objection, not a formation mechanism.
- Generic crucified man: **possible in principle**, but the joint forensic pattern (thorn cap + side wound without crurifragium + hasty linen shroud + no decomposition) is historically rare.
- Jesus of Nazareth as described in the Gospels: **best-fit named candidate** once L1–L4 are granted and L5 is allowed to name a person.

That last step is historical inference, not chemistry.
