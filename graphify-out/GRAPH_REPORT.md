# Graph Report - D.N.E.E  (2026-11-03)

## Corpus Check
- Corpus is ~5,761 words - fits in a single context window. You may not need a graph.

## Summary
- 28 nodes · 33 edges · 5 communities (3 shown, 2 thin omitted)
- Extraction: 97% EXTRACTED · 3% INFERRED · 0% AMBIGUOUS · INFERRED: 1 edges (avg confidence: 0.85)
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- Guia e publicação
- Fluxo e documentos
- Regras e incerteza
- Mapa do cérebro
- Descoberta do projeto

## God Nodes (most connected - your core abstractions)
1. `Framework D.N.E.E. Docs` - 12 edges
2. `Graphify` - 7 edges
3. `Guia interativo` - 6 edges
4. `visao-projeto.html` - 4 edges
5. `Especificar` - 3 edges
6. `SDD.md` - 3 edges
7. `Site ao vivo` - 3 edges
8. `Descobrir` - 2 edges
9. `Nortear` - 2 edges
10. `Evidenciar` - 2 edges

## Surprising Connections (you probably didn't know these)
- `Deploy GitHub Pages` --conceptually_related_to--> `Site ao vivo`  [INFERRED]
  .github/workflows/pages.yml → README.md
- `Mapa do cérebro` --references--> `Graphify`  [EXTRACTED]
  index.html → README.md
- `Guia interativo` --references--> `Framework D.N.E.E. Docs`  [EXTRACTED]
  index.html → README.md
- `Site ao vivo` --references--> `Guia interativo`  [EXTRACTED]
  README.md → index.html

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **Fluxo D.N.E.E.** — readme_descobrir, readme_nortear, readme_especificar, readme_evidenciar [EXTRACTED 1.00]
- **Estrutura de documentação** — readme_cursorrules, readme_visao_projeto_html, readme_sobre_md, readme_sdd_md, readme_roadmap_md, readme_changelog_evidences_md [EXTRACTED 1.00]
- **Protocolo de incerteza** — readme_a_validar, readme_pergunta_ao_responsavel, readme_hipotese_confirmar, readme_pontos_a_complementar [EXTRACTED 1.00]

## Communities (5 total, 2 thin omitted)

### Community 0 - "Guia e publicação"
Cohesion: 0.29
Nodes (7): Deploy GitHub Pages, copyToClipboard, Guia interativo, Mapa do cérebro, switchTab, toggleTheme, Site ao vivo

### Community 1 - "Fluxo e documentos"
Cohesion: 0.33
Nodes (4): CHANGELOG_EVIDENCES.md, ROADMAP.md, SDD.md, visao-projeto.html

### Community 3 - "Mapa do cérebro"
Cohesion: 0.33
Nodes (6): graph.html, graph.json, GRAPH_REPORT.md, Graphify, graphify.mdc, .graphifyignore

## Knowledge Gaps
- **10 isolated node(s):** `.cursorrules`, `switchTab`, `copyToClipboard`, `toggleTheme`, `Deploy GitHub Pages` (+5 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 14 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **2 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `Framework D.N.E.E. Docs` connect `Regras e incerteza` to `Guia e publicação`, `Fluxo e documentos`, `Mapa do cérebro`, `Descoberta do projeto`?**
  _High betweenness centrality (0.774) - this node is a cross-community bridge._
- **What connects `.cursorrules`, `switchTab`, `copyToClipboard` to the rest of the system?**
  _10 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Why does `Graphify` connect `Mapa do cérebro` to `Guia e publicação`, `Regras e incerteza`?**
  _High betweenness centrality (0.363) - this node is a cross-community bridge._
- **Why does `Guia interativo` connect `Guia e publicação` to `Regras e incerteza`?**
  _High betweenness centrality (0.241) - this node is a cross-community bridge._