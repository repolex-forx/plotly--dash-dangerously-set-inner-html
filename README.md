# Repolex Knowledge Graph of plotly/dash-dangerously-set-inner-html

RDF knowledge graph data for [plotly/dash-dangerously-set-inner-html](https://github.com/plotly/dash-dangerously-set-inner-html), parsed by [repolex](https://repolex.ai).

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
rlex download plotly/dash-dangerously-set-inner-html
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 15f7dc7fc4bd08e06f4f9731c247afebdef4051e
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 15f7dc7fc4bd08e06f4f9731c247afebdef4051e
│           └── chunk-001.nq.gz
├── blob
│   ├── 0bf77501804861ef4ea39b5bc728e8aaf7097889.nq.gz
│   ├── 0c305818b3fd759af2366cd2046309f5911494fc.nq.gz
│   ├── 177d39ef54d03a868f942ac8b961eafd635b6647.nq.gz
│   ├── 18d12cfe42742743f9cd4d5a567e90ef3196f14d.nq.gz
│   ├── 29a14acbb0691f6395d402d2c95504c26a731b97.nq.gz
│   ├── 5714e06781976fcc45a44428010df4fd0f706da5.nq.gz
│   ├── 59a47e2aeea1668f98b6d78a41a69784735971ab.nq.gz
│   ├── 6e5a5323fce38a29805a993d06d8ce585bebb14b.nq.gz
│   ├── 71d9a95c8dedf68801d6dcf6387f38ad0384a1a2.nq.gz
│   ├── 7f669a727dda15d849a4637023ee362e953ec852.nq.gz
│   ├── 859fe0c9c855809071dc6410218c59ea6de66350.nq.gz
│   ├── 8cf7af30d0a91e6de7916174ff91ac8d28d5f2a5.nq.gz
│   ├── b1fd20c1356f17037eedacdb734ff7dffc539ae4.nq.gz
│   ├── b2d024ad1dbb0bcf6d6acd7009f7ae7517e2904a.nq.gz
│   ├── bc8371522911dae5c57fa15028a9c84eeb316709.nq.gz
│   ├── cd8c47d3d7e46ef695ddb5cc3b9c2d4dfc633d8d.nq.gz
│   ├── dbd8407b1d2e6d9b101b58913a0e8fb8b44a674f.nq.gz
│   ├── dc6a6f3bb238b883feeb9a6ca99ef461533d96f4.nq.gz
│   ├── e7d1d6f448499cc17acb592f14b6cd6fc5e711d3.nq.gz
│   └── ffcc925ae2ade5f8b863840f7c8a0e337341410c.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 15f7dc7fc4bd08e06f4f9731c247afebdef4051e.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 28 files
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

[plotly/dash-dangerously-set-inner-html](https://github.com/plotly/dash-dangerously-set-inner-html)

---
*Parsed on 2026-11-07 by [repolex](https://repolex.ai)*
