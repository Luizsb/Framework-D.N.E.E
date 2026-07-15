# Framework D.N.E.E.

**Descobrir · Nortear · Especificar · Evidenciar**

Guia interativo para desenvolvimento assistido por IA **sem perder contexto, arquitetura nem rastreabilidade**.

---

## O que é o D.N.E.E.?

O **D.N.E.E.** é um framework leve de governança para projetos com IA (Cursor, Copilot e similares).

A IA acelera a escrita de código, mas sem processo isso gera **perda de contexto** e **arquitetura espaguete**. O D.N.E.E. transferre o fardo da documentação para a própria IA, com um fluxo mínimo e obrigatório:

| Etapa | Significado | O que acontece |
|-------|-------------|----------------|
| **D** | Descobrir | A IA avalia o problema, levanta hipótese de valor e propõe a solução **antes** de tocar no código |
| **N** | Nortear | A IA consulta o **Documento Norte (SDD)** para respeitar regras e arquitetura vigentes |
| **E** | Especificar | A solução vira tarefas claras (roadmap / checklists) para execução controlada |
| **E** | Evidenciar | Após o sucesso, a IA registra **Antes, Depois e Decisão** no changelog de evidências |

É o **mínimo viável perfeito**: pouca cerimônia, muita clareza.

---

## O que tem neste repositório

| Arquivo | Descrição |
|---------|-----------|
| [`guia_definitivo_d_n_e_e.html`](./guia_definitivo_d_n_e_e.html) | Página interativa completa do framework — conceito, arquitetura de arquivos, mega-prompts e rotina do dia a dia |
| [`index.html`](./index.html) | Mesma página, publicada no GitHub Pages |

**Site ao vivo:** [https://luizsb.github.io/Framework-D.N.E.E/](https://luizsb.github.io/Framework-D.N.E.E/)

Abra o HTML no navegador (ou o link acima) para navegar pelo guia (conceito, estrutura, aplicação em projetos novos/legados e operação diária).

---

## A estrutura de arquivos (o Canvas)

A regra de ouro: **a fonte da verdade deve ser condensada e visual**. Em vez de dezenas de pastas soltas, o D.N.E.E. usa poucos elementos-chave:

```text
meu-projeto/
├── .cursorrules              ← A Constituição (obriga o fluxo D.N.E.E.)
├── docs/
│   ├── visao-projeto.html    ← Dashboard visual (para humanos)
│   ├── SOBRE.md              ← Pitch de negócio (porta de entrada)
│   ├── SDD.md                ← Norte técnico (arquitetura + regras)
│   ├── ROADMAP.md            ← Futuro (fases, débitos, tarefas)
│   └── CHANGELOG_EVIDENCES.md← Passado (evidências com data/hora)
└── src/
    └── ...                   ← Seu código
```

| Artefato | Papel |
|----------|--------|
| `.cursorrules` | Constituição: força a IA a seguir D.N.E.E., pensar como PM e formatar a documentação |
| `visao-projeto.html` | UI em abas que renderiza os Markdown para gestores, QA e o time |
| `SOBRE.md` | Visão de negócio em linguagem leiga (problema, público, valor) |
| `SDD.md` | Verdade técnica absoluta — arquitetura e regras inquebráveis |
| `ROADMAP.md` | Planejamento, débitos técnicos e próximas tarefas |
| `CHANGELOG_EVIDENCES.md` | Histórico de valor gerado no formato `AAAA-MM-DD · HH:MM — Mudança` |

---

## Para quem é

- Times que usam IA no dia a dia e precisam de **controle e memória**
- Projetos **novos** (nascem com governança) e **legados** (primeiro mapeiam a realidade, depois documentam)
- Stakeholders que querem ver o projeto sem abrir o código

---

## Como começar

1. Abra [`guia_definitivo_d_n_e_e.html`](./guia_definitivo_d_n_e_e.html) no navegador
2. Vá em **Como Aplicar**
3. Copie o **Mega-Prompt** (projeto novo ou legado) e cole no Cursor
4. Deixe a IA montar a estrutura `docs/` + `.cursorrules` e siga o fluxo D.N.E.E. em toda feature

---

## Princípio

> Documentação não é burocracia paralela — é o **contexto oficial** que a IA lê antes de mudar o sistema e registra depois de entregar valor.

---

## Licença

Uso livre para projetos pessoais e profissionais. Adapte o canvas e os prompts à sua realidade.
