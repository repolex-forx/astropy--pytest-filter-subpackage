# Repolex Knowledge Graph of astropy/pytest-filter-subpackage

RDF knowledge graph data for [astropy/pytest-filter-subpackage](https://github.com/astropy/pytest-filter-subpackage), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download astropy/pytest-filter-subpackage
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 30737bed6bbe975a3e65d2f439eec296e9e4d990
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 30737bed6bbe975a3e65d2f439eec296e9e4d990
│           └── chunk-001.nq.gz
├── blob
│   ├── 0791e17492026aa473ce703250a634d3a1d67eda.nq.gz
│   ├── 210f76a3aac88c17cab287eda774effb2378ecdf.nq.gz
│   ├── 27355f916a9851d75addaee33b50e6000921b146.nq.gz
│   ├── 2c5f2d8ee35de89bbacabad5420e3a79bee22025.nq.gz
│   ├── 3ba20b6a835f8cf93ab46759ab9b0741a329cb42.nq.gz
│   ├── 8001e2590cab798bb189d31650e4f7dc6a132277.nq.gz
│   ├── 8aaf03e3f5def297a66688e1339a297b8e980a05.nq.gz
│   ├── 8b8ebcc690eccac11585517c67b0af23b63cf444.nq.gz
│   ├── a5d123cb970f717d48b838b897c887af778e7da5.nq.gz
│   ├── a63fbf585e689345613bc522010bdfacd55d6e74.nq.gz
│   ├── b507b35474ebf2eb9aeb41a0a0b918e0c6c1464b.nq.gz
│   ├── d05628a081046c895ba3b56594d2ffb6ffb4891c.nq.gz
│   ├── da0d502748620c87a4819f9ad64552fced280431.nq.gz
│   ├── dc7563f1916435b9f5a5d4b8433355085ddc0862.nq.gz
│   ├── ec8a646cbee9bc34ebb8bfb9e070376224117cfd.nq.gz
│   └── f207ee564e97876c41045bdccb2fa245d7b51872.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 30737bed6bbe975a3e65d2f439eec296e9e4d990.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 24 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[astropy/pytest-filter-subpackage](https://github.com/astropy/pytest-filter-subpackage)

---
*Parsed on 2026-10-21 by [repolex](https://repolex.ai)*
