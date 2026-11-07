# Fundamentos de Engenharia de IA

Pesquisa em grupo do **Hype Data & AI** · **Área de estudo:** Agentes/LLMs

## Integrantes
- Gabriel Fernandes Marchesano
- Enzo Henrique Dias Ribeiro
- Erick Belleza Spina
- Juliana Kaori Suzuki

**Coordenador(es):** _a definir_

---

## 1. Introdução

### 1.1. Descrição do tema
A área de **Engenharia de IA** consiste na aplicação de práticas rigorosas de engenharia de software para projetar, orquestrar e sustentar aplicações baseadas em Grandes Modelos de Linguagem (LLMs). O projeto aborda o ciclo completo de desenvolvimento dessas soluções, cobrindo desde a parametrização de APIs e Engenharia de Prompt até a construção de Agentes de IA autônomos capacitados com ferramentas (*Function Calling*), arquiteturas avançadas de Recuperação Aumentada por Geração (como *Agentic RAG* e *Graph RAG*) e a criação de AI Harnesses para testes automatizados (*Evals*), observabilidade e segurança de dados.

O mercado vem passando por uma transição de protótipos de chat para sistemas cognitivos integrados em produção. Isso ajuda as empresas que buscam adotar a IA a mitigar o não-determinismo e as alucinações dos modelos, conectar LLMs a bases de dados corporativas em tempo real sem re-treinamentos custosos, automatizar fluxos operacionais complexos de ponta a ponta e garantir governança por meio de métricas claras de desempenho, latência e custo.

### 1.2. Objetivos da documentação
- Apresentar e descrever as principais técnicas que envolvem chamadas de LLMs e a criação de agentes de IA que usam esses modelos.

---

## 2. Plano de estudo e pesquisa

### 2.1. Estrutura de conteúdo

| # | Tópico | Conteúdo |
|---|--------|----------|
| 1 | [Fundamentos de LLMs e Chamadas de API](etapa-1-capitulos-1-e-2/01-fundamentos-llms-chamadas-api/) | Parâmetros de modelos (`temperature`, `top_p`, `frequency_penalty`, `max_tokens`); papéis System/User/Assistant; saídas estruturadas (JSON) |
| 2 | [Engenharia de Prompt e Gerenciamento de Contexto](etapa-1-capitulos-1-e-2/02-engenharia-prompt-contexto/) | Zero-shot, Few-shot, Chain-of-Thought, ReAct; sumarização dinâmica, truncation e compressão de histórico |
| 3 | [RAG (Retrieval-Augmented Generation)](etapa-2-rag/03-rag/) | Chunking e embeddings; Vector DBs; RAG vs Fine-Tuning; grafos de conhecimento |
| 4 | [Agentes de IA e Uso de Ferramentas](etapa-3-capitulos-4-e-5/04-agentes-ia-ferramentas/) | Conceito de agente; Function Calling & Tools; Agentic RAG; orquestração multi-agente |
| 5 | [Tópicos Avançados](etapa-3-capitulos-4-e-5/05-topicos-avancados/) | AI Harness e Evaluation Harness; segurança; observabilidade |

### 2.2. Metodologia de pesquisa
_A definir._

---

## 3. Divisão de etapas e entregas

> ⚠️ **Todas as datas abaixo estão sujeitas a alteração.** Elas seguem o planejamento inicial e serão atualizadas aqui conforme mudarem.

**Forma de entrega:** cada etapa deve ser entregue para o email **hype-each@usp.br** com o assunto `Nome Do Projeto - Etapa X`, anexando o documento da pesquisa (com exceção da Etapa 0).

| Etapa | Descrição | Data* | Pasta |
|-------|-----------|-------|-------|
| 0 | Definição de grupos e preenchimento do template de planejamento | 27/09 | [etapa-0-definicao-de-grupos/](etapa-0-definicao-de-grupos/) |
| 1 | Tópicos/Capítulos 1 e 2 — notebooks sobre boas práticas de prompt e contexto, com aplicações simples de exemplo | 17/10 | [etapa-1-capitulos-1-e-2/](etapa-1-capitulos-1-e-2/) |
| 2 | RAG (Capítulo 3) — pipeline RAG simples (chunking, embeddings, banco vetorial, recuperação e geração), comparação RAG vs fine-tuning e evolução da técnica | 07/11 | [etapa-2-rag/](etapa-2-rag/) |
| 3 | Tópicos/Capítulos 4 e 5 — agente de IA simples para uma funcionalidade X e início da documentação de tópicos avançados | 05/12 | [etapa-3-capitulos-4-e-5/](etapa-3-capitulos-4-e-5/) |
| 4 | Documentação completa (Harness) + artigo na Newsletter sobre uma técnica do estado da arte | 27/02 (a depender do período de férias do Hype) | [etapa-4-documentacao-completa-artigo/](etapa-4-documentacao-completa-artigo/) |

\* Datas sujeitas a alteração.

---

## 4. Estrutura do repositório

```
fundamentos-engenharia-ia/
├── README.md
├── etapa-0-definicao-de-grupos/
├── etapa-1-capitulos-1-e-2/
│   ├── 01-fundamentos-llms-chamadas-api/
│   │   ├── README.md
│   │   ├── REFERENCIAS.md
│   │   └── notebooks/
│   └── 02-engenharia-prompt-contexto/
├── etapa-2-rag/
│   └── 03-rag/
├── etapa-3-capitulos-4-e-5/
│   ├── 04-agentes-ia-ferramentas/   (código em agente/)
│   └── 05-topicos-avancados/
└── etapa-4-documentacao-completa-artigo/
    ├── documentacao-harness/
    └── artigo-newsletter/
```

Cada tópico tem seu próprio `README.md` (visão geral e andamento) e seu próprio `REFERENCIAS.md` (artigos, livros e materiais usados como base).

---

## 5. Referências bibliográficas

As referências ficam organizadas por tópico, no arquivo `REFERENCIAS.md` de cada pasta:

- [1. Fundamentos de LLMs e Chamadas de API](etapa-1-capitulos-1-e-2/01-fundamentos-llms-chamadas-api/REFERENCIAS.md)
- [2. Engenharia de Prompt e Gerenciamento de Contexto](etapa-1-capitulos-1-e-2/02-engenharia-prompt-contexto/REFERENCIAS.md)
- [3. RAG](etapa-2-rag/03-rag/REFERENCIAS.md)
- [4. Agentes de IA e Uso de Ferramentas](etapa-3-capitulos-4-e-5/04-agentes-ia-ferramentas/REFERENCIAS.md)
- [5. Tópicos Avançados](etapa-3-capitulos-4-e-5/05-topicos-avancados/REFERENCIAS.md)
- [Etapa 4 — Documentação de Harness](etapa-4-documentacao-completa-artigo/documentacao-harness/REFERENCIAS.md)
- [Etapa 4 — Artigo para a Newsletter](etapa-4-documentacao-completa-artigo/artigo-newsletter/REFERENCIAS.md)
