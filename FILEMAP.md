# Filemap · content-areas

> **What is this file?** A living snapshot of this repo's directory shape: top-level dirs annotated for purpose, plus an auto-generated tree. Maintained per the `maintain-filemap` loop, with the same override as the parent `content` repo: the tree is **directories only** (`tree -d`), because a file-inclusive tree is mostly a long list of organization names rather than a map. Regenerate via:
>
> ```bash
> tree -L 3 -d -I 'node_modules|.git|.DS_Store|.claude' --noreport --dirsfirst . | tr '\240' ' '
> ```
>
> then splice the output between the sentinels below. (The `tr` swaps the non-breaking spaces `tree` emits for plain ones, so regenerations don't produce whitespace-only diffs.)

This repo is a git submodule of [`lossless-content`](https://github.com/lossless-group/lossless-content), mounted at `content/content-areas/`. See `README.md` for what a content area is and how to contribute.

## Top-level directories

| Path | What it is |
|---|---|
| `AI-Factories-Datacenters` | AI factories and datacenters: operators, builders, power, grid, cooling, financing (started October 2026) |
| `Blue-Economy` | Water, sustainability, ocean and water-innovation organizations and issues |
| `Finance` | Finance content area; currently organized by sub-domain (`Private-Markets/`) rather than the standard folder set |
| `Health` | Healthcare, public health, HealthTech, medicine |
| `general` | Lowercase, cross-area folder: shared documents that render in any area, and a catch-all when placement is unclear |
| `changelog` | Dated ship log for this repo |

Capitalized folders are content areas; lowercase folders are shared. Each area aims for the same subfolders: `Organizations/`, `Concepts/`, `Topics/`, `Issues/`, `Vocabulary/`, `Sources/`.

## Shape notes (as of 2026-10-04)

Places where the tree differs from that convention, recorded here rather than fixed:

- `Finance/` nests under `Private-Markets/` instead of using the standard subfolders at its root.
- `Health/` has no subfolders yet (4 files at its root).
- `general/` has no `sources/` folder.
- `Cusp AI.md` and `Luminance.md` sit at the repo root rather than inside an area.
- `AI-Factories-Datacenters/Oracle Cloud Infrastructure.md` sits at the area root rather than in `Organizations/`.

## Tree (directories, depth 3, auto-generated)

<!-- TREE-START -->
```
.
├── AI-Factories-Datacenters
│   ├── Concepts
│   ├── Issues
│   ├── Organizations
│   ├── Sources
│   ├── Topics
│   └── Vocabulary
├── Blue-Economy
│   ├── Concepts
│   ├── Issues
│   ├── Organizations
│   ├── Sources
│   ├── Topics
│   └── Vocabulary
├── changelog
├── Finance
│   └── Private-Markets
│       └── Concepts
├── general
│   ├── concepts
│   ├── issues
│   ├── organizations
│   ├── topics
│   └── vocabulary
└── Health
```
<!-- TREE-END -->
