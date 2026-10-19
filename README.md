# Repolex Knowledge Graph of ionelmc/python-manhole

RDF knowledge graph data for [ionelmc/python-manhole](https://github.com/ionelmc/python-manhole), parsed by [repolex](https://repolex.ai).

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
rlex download ionelmc/python-manhole
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 175f426fc4794ae9a54f9daba032e3e5631e7db3
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 175f426fc4794ae9a54f9daba032e3e5631e7db3
│           └── chunk-001.nq.gz
├── blob
│   ├── 009a913cde5985359d40200f00c0efcc2baf5582.nq.gz
│   ├── 0d46798d39a7dc082169962b89b1c9e073028923.nq.gz
│   ├── 0e727ce3529b276a3ab7a7df899599f8dc7dafdb.nq.gz
│   ├── 156f8e535b2ec351d1e0f36ca69695aa6c8da5a8.nq.gz
│   ├── 15ae905688c940e580e057b04ce5c27764d76f27.nq.gz
│   ├── 201bb28eaa61cb07957ff4e8d146a4e5de75bff5.nq.gz
│   ├── 2ae3ccff66cd4aceddbd0b38dd6a880f52abe1f4.nq.gz
│   ├── 38fac2841848354e3d59f888d83ae123159354b1.nq.gz
│   ├── 3c03dfbe8ff859a96cc37073c7a2a13959a6210c.nq.gz
│   ├── 4421ff4f504af272a18ab098337ffbbc08939404.nq.gz
│   ├── 48c8347a1fc23de3fdcb2aeb024bdaa63040f68d.nq.gz
│   ├── 565b0521d0c2cdbfe493d19765b04d5c119fa7eb.nq.gz
│   ├── 586c7367de1cff5d362be309c0a4014b0905edb1.nq.gz
│   ├── 6f589ef040f8edc17b405aff7953728de7561c79.nq.gz
│   ├── 72a33558153fb57def85612b021ec596ef2a51b9.nq.gz
│   ├── 770e36ed77519bd8b5250531a3cd986f5cf185fa.nq.gz
│   ├── 77973dd9ff9648541ba9872375bba8ed6e340038.nq.gz
│   ├── 7c54c323de59f1a5813ddd0333ebaf7214498546.nq.gz
│   ├── 94462ce67a0670b337ec933f38882693f8debe00.nq.gz
│   ├── a1708f401aa3b38d34cfb9a7b6d084fce2014e32.nq.gz
│   ├── a94792e98bea65c9772ef5d26a15d0b0dd76dcd5.nq.gz
│   ├── a95f2e5764de3fa96aa7f0ea3b814b3a754fc402.nq.gz
│   ├── ad842d51d97d389707466a2f855e895fa0b9f6d6.nq.gz
│   ├── afdc4ad6d8e3354427bd37d9207b30dd63185855.nq.gz
│   ├── b86eb4f8b467104b37527d33d9012cd912bfafd8.nq.gz
│   ├── b9f149672422af233578a36ffb1ee9f7b5eaaeac.nq.gz
│   ├── c03e307ab39cd6807b9bc0d8f404e716707c2533.nq.gz
│   ├── cd1cddcc458a6c6752e2e8ecb5039caf2e0b1ca0.nq.gz
│   ├── d0dac9c381161c95e487044411c1f9838f4ffe3a.nq.gz
│   ├── d3178deb6e8d2f1855a87481a9f3a05ebbea51b7.nq.gz
│   ├── d71a3584d8225bde4c43bbef3f7ea2c0290bb515.nq.gz
│   ├── dbe8c41f2a3899906af6223b61b8ce77e7bc20de.nq.gz
│   ├── dcb6755a32867d2dcc45158990d770ec784375b3.nq.gz
│   ├── dceea2bfe05a0ee09a129dacc3f7c29befb29ed5.nq.gz
│   ├── e122f914a87b277e565fc9567af1a7545ec9872b.nq.gz
│   ├── e3a6b3c723c3f8cf2d2dfbdd66988760961b242c.nq.gz
│   ├── e582053ea018c369be05aae96cf730744f1dc616.nq.gz
│   ├── ecb518021bde10e7b6635f8292ef8237642f1d5a.nq.gz
│   ├── f170cf5b4378615a9f8cb5dfdbaaaef21cce00a3.nq.gz
│   ├── f3c9a7ea683e2a0b79a04e03b91fa117b49a08b0.nq.gz
│   └── f95eb78d8a603b0fe5d17560d0dd04877d55c71c.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 175f426fc4794ae9a54f9daba032e3e5631e7db3.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 49 files
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

[ionelmc/python-manhole](https://github.com/ionelmc/python-manhole)

---
*Parsed on 2026-10-19 by [repolex](https://repolex.ai)*
