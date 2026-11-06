# Repolex Knowledge Graph of tcmetzger/sphinx-favicon

RDF knowledge graph data for [tcmetzger/sphinx-favicon](https://github.com/tcmetzger/sphinx-favicon), parsed by [repolex](https://repolex.ai).

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
rlex download tcmetzger/sphinx-favicon
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 95a723a0fe71a26d110b671854d6bc8e87d1c850
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 95a723a0fe71a26d110b671854d6bc8e87d1c850
│           └── chunk-001.nq.gz
├── blob
│   ├── 07c088ba43120d7d78312219695b91b01317000d.nq.gz
│   ├── 087cc135476a1f1aa2fdff30da626bf4d9b058aa.nq.gz
│   ├── 19d509263c0504677b626a34f0b5193e76c7f787.nq.gz
│   ├── 1adb4343d8520cbe560203c2d899b0687ce756c9.nq.gz
│   ├── 338805e4ee74dd2ff49ce010405fb89ad7b49da3.nq.gz
│   ├── 3c197ec4e9362fdd22757948534e080ed4b34894.nq.gz
│   ├── 3d66215af2f06cb1238cfff2448ed35be8db2996.nq.gz
│   ├── 40c0649fff5e819a06154b854ac8da7656b3734a.nq.gz
│   ├── 4b07a89f5cda610619845e1e2f4c14d5b5790350.nq.gz
│   ├── 547054c9015a329bb4766d9138b178d94ec0312b.nq.gz
│   ├── 56357a71978b8c5a67db59c046b1093b75164ae4.nq.gz
│   ├── 64192c14b3d16c647f9f19cdf61a3be85120e876.nq.gz
│   ├── 6d8778b595addb7dc60c89e93c8bd37a2dccd35b.nq.gz
│   ├── 718485bd4939597e6315a93011b461b176e668e0.nq.gz
│   ├── 7c5ea809b6df6ef1ac12395ab0cb43facc03c767.nq.gz
│   ├── 88c341845e93251dce5d558065760abc2289df50.nq.gz
│   ├── 8aad69bb2fa105afee4c96f527effac209d9023b.nq.gz
│   ├── 8b137891791fe96927ad78e64b0aad7bded08bdc.nq.gz
│   ├── 90b8e267ca141f240f0a9605b69721a762b3184e.nq.gz
│   ├── 9d7f76c936de4140f730ec33f9d333b173f0976c.nq.gz
│   ├── a17dedc0247f0dded5ed89ff2c47bcfabaede769.nq.gz
│   ├── a6072b454ee130f6f9e3d958d60237a075795921.nq.gz
│   ├── a697ae3702c2f649a5a082442da812e5fbcef664.nq.gz
│   ├── a9a4d3e9aa1d98694e974568e5652731eb35d8d4.nq.gz
│   ├── b30d5642364ebfeae9947cdb07583ecc398cccfa.nq.gz
│   ├── b908cbe55cb344569d32de1dfc10ca7323828dc5.nq.gz
│   ├── be4f1f44eb6d3ece5f5ee8accceaa03e55c7af11.nq.gz
│   ├── c09f8b61d1f5716b08b823f2777e8def41ee37cd.nq.gz
│   ├── c0f08bd768593c37c4c8b7ff013ba6061cac5426.nq.gz
│   ├── c662f148d36f1a167cda6bdec09a70b11cc2f64f.nq.gz
│   ├── ca29bc5ceb948b44ab6babff59bfc75ddef8c23e.nq.gz
│   ├── d200f090996adbc21180c30d87584a768ee9ac40.nq.gz
│   ├── d54fc8c1a22dd8fe286548bf1d8b04faa51e3c2f.nq.gz
│   ├── d5b2566c3a571767109e05f6e026b45e72ccbf1a.nq.gz
│   ├── d76986fea1941c8ebdd01f68753328bc426f33d1.nq.gz
│   ├── dbf79f3879517ce9c95a25fe3ee588bbdf157806.nq.gz
│   ├── dfd876726d6c68a45893b0d8cd8f5f3348dc1c03.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── eed02d3ccf95da4962e8cfcd288bccbf9fb62005.nq.gz
│   ├── f008a6b98731ad809f9c33276203bcfbf92d7ca4.nq.gz
│   └── f319efa4d0ffd5bbb5831f6d5a81a928f4422b30.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 95a723a0fe71a26d110b671854d6bc8e87d1c850.nq.gz
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

[tcmetzger/sphinx-favicon](https://github.com/tcmetzger/sphinx-favicon)

---
*Parsed on 2026-11-06 by [repolex](https://repolex.ai)*
