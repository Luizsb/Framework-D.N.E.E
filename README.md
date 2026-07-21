# Framework D.N.E.E. Docs

**Descobrir · Nortear · Especificar · Evidenciar**

Um processo leve para documentar, evoluir e manter projetos com apoio de IA — **sem perder contexto, arquitetura nem rastreabilidade**.

---

## O que é o D.N.E.E. Docs?

O **D.N.E.E. Docs** é um padrão leve de documentação viva para projetos com IA (Cursor, Copilot e similares).

A IA acelera a criação de código, mas sem documentação viva ela também pode gerar **perda de contexto, decisões soltas e retrabalho**. O D.N.E.E. Docs cria um fluxo simples para descobrir o problema, nortear o projeto, planejar mudanças e registrar evidências:

| Etapa | Significado | O que acontece |
|-------|-------------|----------------|
| **D** | Descobrir | A IA avalia o problema, levanta hipótese de valor e propõe a solução **antes** de tocar no código |
| **N** | Nortear | A IA consulta o **Norte do projeto (SDD.md)** para respeitar regras e arquitetura vigentes |
| **E** | Especificar | A solução vira tarefas claras no `ROADMAP.md` e critérios de aceite no `SDD.md` antes de gerar código |
| **E** | Evidenciar | Após o sucesso, a IA registra **Antes, Depois e Decisão** no `CHANGELOG_EVIDENCES.md` |

É o **mínimo viável perfeito**: pouca cerimônia, muita clareza.

---

## O que tem neste repositório

| Arquivo | Descrição |
|---------|-----------|
| [`index.html`](./index.html) | Guia interativo do padrão — conceito, estrutura, prompts prontos e rotina do dia a dia (com modo claro/escuro) |

**Site ao vivo:** [https://luizsb.github.io/Framework-D.N.E.E/](https://luizsb.github.io/Framework-D.N.E.E/)

Abra o HTML no navegador (ou o link acima) para navegar pelo guia (conceito, estrutura, aplicação em projetos novos/legados e operação diária).

---

## A estrutura de arquivos

A regra de ouro: **a fonte da verdade são os arquivos Markdown** dentro de `docs/`. A página `visao-projeto.html` é apenas a interface visual para leitura humana. Nada além disso é obrigatório:

```text
meu-projeto/
├── .cursorrules              ← A Constituição (obriga o fluxo D.N.E.E. Docs)
├── docs/
│   ├── visao-projeto.html    ← Interface visual (para humanos)
│   ├── SOBRE.md              ← Pitch de negócio (porta de entrada)
│   ├── SDD.md                ← Norte técnico (arquitetura + regras)
│   ├── ROADMAP.md            ← Futuro (fases, débitos, tarefas)
│   └── CHANGELOG_EVIDENCES.md← Passado (decisões e evidências)
└── src/
    └── ...                   ← Seu código
```

| Artefato | Papel |
|----------|--------|
| `.cursorrules` | Constituição: força a IA a seguir o D.N.E.E. Docs, pensar como PM e manter a documentação atualizada |
| `visao-projeto.html` | UI com exatamente 4 abas que renderiza os Markdown para gestores, QA e o time |
| `SOBRE.md` | Visão de negócio em linguagem leiga (problema, público, valor e Discovery resumido) |
| `SDD.md` | Verdade técnica — escopo, fluxos, arquitetura, regras e critérios de qualidade |
| `ROADMAP.md` | Planejamento, backlog priorizado, débitos técnicos e próximas ações |
| `CHANGELOG_EVIDENCES.md` | Histórico de decisões e valor gerado no formato `AAAA-MM-DD · HH:MM — Mudança` |

**As 4 abas da documentação visual:** 💡 Sobre o projeto · 🧭 Norte do projeto · 🗺️ Roadmap · 📌 Decisões & Evidências

> **Camada opcional:** para projetos muito grandes, com múltiplos devs ou necessidade de specs formais, o time pode adicionar uma pasta extra de especificações. No fluxo padrão, o D.N.E.E. Docs funciona apenas com a pasta `docs/`.

---

## Quando a IA não souber algo

A IA não deve inventar informações para parecer completa. Toda incerteza usa marcações padronizadas:

- `[A VALIDAR]` — informação que precisa ser confirmada
- `[PERGUNTA AO RESPONSÁVEL]` — precisa de resposta humana para continuar
- `[HIPÓTESE — CONFIRMAR]` — hipótese provável, mas não validada

Todo arquivo Markdown termina com uma seção **"Pontos a complementar"** — a documentação nunca fica falsa, fica viva.

---

## Para quem é

- Times que usam IA no dia a dia e precisam de **controle e memória**
- Projetos **novos** (nascem com governança) e **legados** (primeiro mapeiam a realidade, depois documentam)
- Stakeholders que querem ver o projeto sem abrir o código

---

## Como começar

1. Abra [`index.html`](./index.html) no navegador (ou o [site ao vivo](https://luizsb.github.io/Framework-D.N.E.E/))
2. Vá em **Como Aplicar**
3. Copie o prompt de **Projeto Novo** ou **Projeto Existente** e cole no Cursor
4. Deixe a IA fazer o Discovery, montar a estrutura `docs/` + `.cursorrules` e siga o fluxo D.N.E.E. Docs em toda mudança relevante

---

## Princípio

> Documentação não é burocracia paralela — é o **contexto oficial** que a IA lê antes de mudar o sistema e registra depois de entregar valor.

---

## Créditos

Criado e mantido por **Luiz Stival** · Time **Interações Digitais**.

Feedback, ajustes ou melhorias? [Fale comigo no Slack](https://arco.enterprise.slack.com/team/U0830TU216H).

---

## Licença

Uso livre para projetos pessoais e profissionais. Adapte a estrutura e os prompts à sua realidade.
