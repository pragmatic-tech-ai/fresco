# Graph Report - Fresco  (2026-10-04)

## Corpus Check
- 110 files · ~38,577 words
- Verdict: corpus is large enough that graph structure adds value.
- Unclassified: 4 file(s) not represented in the graph (top: (none) 4)

## Summary
- 37 nodes · 36 edges · 6 communities (5 shown, 1 thin omitted)
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `84430d5b`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- package.json
- scripts
- devDependencies
- dependencies
- publishConfig
- engines

## God Nodes (most connected - your core abstractions)
1. `scripts` - 8 edges
2. `publishConfig` - 3 edges
3. `engines` - 2 edges
4. `main` - 1 edges
5. `types` - 1 edges
6. `exports` - 1 edges
7. `files` - 1 edges
8. `registry` - 1 edges
9. `access` - 1 edges
10. `build` - 1 edges

## Surprising Connections (you probably didn't know these)
- None detected - all connections are within the same source files.

## Import Cycles
- None detected.

## Communities (6 total, 1 thin omitted)

### Community 0 - "package.json"
Cohesion: 0.12
Nodes (15): description, exports, files, license, main, name, type, types (+7 more)

### Community 1 - "scripts"
Cohesion: 0.25
Nodes (8): scripts, build, clean, ge, ge:compound, prepublishOnly, test, typecheck

### Community 2 - "devDependencies"
Cohesion: 0.40
Nodes (5): devDependencies, rimraf, tsx, @types/node, typescript

### Community 3 - "dependencies"
Cohesion: 0.67
Nodes (3): dependencies, @pragmatic-tech-ai/mural, yaml

### Community 4 - "publishConfig"
Cohesion: 0.67
Nodes (3): publishConfig, access, registry

## Knowledge Gaps
- **31 isolated node(s):** `name`, `version`, `description`, `type`, `main` (+26 more)
  These have ≤1 connection - possible missing edges. (Counts symbols only; 31 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **1 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `scripts` connect `scripts` to `package.json`?**
  _High betweenness centrality (0.356) - this node is a cross-community bridge._
- **Why does `devDependencies` connect `devDependencies` to `package.json`?**
  _High betweenness centrality (0.213) - this node is a cross-community bridge._
- **Why does `publishConfig` connect `publishConfig` to `package.json`?**
  _High betweenness centrality (0.110) - this node is a cross-community bridge._
- **What connects `name`, `version`, `description` to the rest of the system?**
  _31 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `package.json` be split into smaller, more focused modules?**
  _Cohesion score 0.125 - nodes in this community are weakly interconnected._