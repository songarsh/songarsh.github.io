# Artifact-evaluation badges

Official ACM and IEEE artifact badges, shown on the right-hand side of a
publication row. Assign them per paper in `_bibliography/papers.bib`:

```bibtex
artifact_badges = {acm-available, acm-functional, acm-reproduced}
```

Keys, display names and links live in `_data/artifact_badges.yml`.

| Key              | Badge                                | Source                             |
| ---------------- | ------------------------------------ | ---------------------------------- |
| `acm-available`  | ACM Artifacts Available              | acm.org, artifact-review v1.1      |
| `acm-functional` | ACM Artifacts Evaluated – Functional | acm.org, artifact-review v1.1      |
| `acm-reusable`   | ACM Artifacts Evaluated – Reusable   | acm.org, artifact-review v1.1      |
| `acm-reproduced` | ACM Results Reproduced               | acm.org, artifact-review v1.1      |
| `acm-replicated` | ACM Results Replicated               | acm.org, artifact-review v1.1      |
| `ieee-oro`       | IEEE Open Research Objects (ORO)     | IEEE camera-ready badge kit (HPCA) |
| `ieee-ror`       | IEEE Research Objects Reviewed (ROR) | IEEE camera-ready badge kit (HPCA) |
| `ieee-ror-r`     | IEEE Results Reproduced (ROR-R)      | IEEE camera-ready badge kit (HPCA) |

## Provenance

The five ACM seals are the publisher's own v1.1 artwork, downloaded from
`https://www.acm.org/binaries/content/gallery/acm/publications/artifact-review-v1_1-badges/`.

The three IEEE pictograms were rendered from the badge PDFs in the HPCA
camera-ready kit (`ae-badges/{open-research-objects,research-objects-reviewed,results-reproduced}.pdf`).

Every file was normalized the same way: trim the transparent margin, scale to
fit a 160×160 transparent square, strip metadata. 160px gives roughly 3×
headroom over the ~40px they render at, so they stay sharp on high-DPI screens.
Keep that geometry when adding a badge, otherwise rows will not line up.

## Adding a badge

Drop the file in this folder, add an entry to `_data/artifact_badges.yml` with
its `name`, `image` and `url`, then reference the new key from a bib entry. No
template change is needed.

- ACM policy: <https://www.acm.org/publications/policies/artifact-review-and-badging-current>
- IEEE badge definitions (NISO RP-31-2021): <https://www.niso.org/publications/rp-31-2021-badging>
