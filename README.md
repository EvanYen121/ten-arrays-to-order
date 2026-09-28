# Ten Arrays to Order

Candidate pentameric guide arrays selected for synthesis — 10 independent elements across 9 VIPR subfamilies. Selection date 2026-09-26.

**Open the report: https://evanyen121.github.io/ten-arrays-to-order/**

`index.html` is a self-contained interactive page — no build step, no dependencies. Clone and open it in a browser, or use the link above.

## The ten elements

| Rank | Element | Contig | VIPR | Unit | Spacers |
|-----:|---------|--------|------|------|--------:|
| 1 | E19 | Ga0456045_0000084 | — | GANNK | 8 |
| 5 | E16 | Ga0137427_10000164 | vipr_c008 | HNNGG | 5 |
| 15 | E11 | Ga0315294_10027407 | vipr_c012 | NNGGC | 19 |
| 22 | E12 | Ga0153916_10000018 | vipr_c004 | NGGMV | 16 |
| 23 | E13 | Ga0453905_0014542 | vipr_c029 | NGGHN | 8 |
| 38 | E01 | Ga0194110_10002104 | vipr_c016 | NNGDT | 3 |
| 41 | E24 | Ga0466548_000010 | vipr_c019 | NGGHN | 6 |
| 43 | E04 | Ga0318466_10102992 | vipr_c018 | YNNGK | 7 |
| 47 | E27 | Ga0247389_10064767 | vipr_iter3 | NNGTD | 20 |
| 50 | E09 | Ga0163144_10003642 | vipr_c020 | NVGVV | 8 |

Ranks are positions in the full screen, not consecutive — these ten were picked for subfamily independence, not by rank alone. E19 carries no VIPR effector hit, which is why ten elements span nine subfamilies.

## Methods

- Grammar computed in spacer-local coordinates on the effector's strand. Elements whose effector sits on the minus strand were flipped before scoring; E19, having no effector, is reported as-deposited.
- Evo 2 tracks from `evo2-40b` forward passes over each array window.
- RNA folding by ViennaRNA `RNAfold -d2`.
- Hairpin z-scores against 200 dinucleotide shuffles.
- Gapless profiles are ungapped self-identity of the concatenated spacers.
