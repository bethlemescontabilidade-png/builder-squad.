# AgencIA 🎯

**Uma agência de marketing completa — em agentes de IA para o Claude Code.**

A AgencIA reúne o melhor de cada disciplina de marketing sob um orquestrador. Você descreve o objetivo e os agentes conduzem a campanha de ponta a ponta, com **workflows pré-definidos**: `mensagem → copy → criativo → distribuição`.

Os agentes não têm nome de pessoa — o nome deles **é a disciplina**.

---

## Instalar

### Opção 1 — Um comando (recomendado)

Cole no seu terminal:

```bash
bash <(curl -sL https://raw.githubusercontent.com/ohmyjahh/AgencIA/main/install.sh)
```

Reinicie o Claude Code. Pronto — digite `@orquestrador` em qualquer projeto.

### Opção 2 — Pelo Claude Code (só o link)

Abra o Claude Code e cole:

> Instale esses agentes globalmente no meu computador, para que eu consiga usar em qualquer chat ou projeto. Quando eu digitar / quero que apareçam os agentes para eu escolher. Segue o link do projeto no GitHub para você instalar: https://github.com/ohmyjahh/AgencIA.git

### Opção 3 — Manual

```bash
git clone https://github.com/ohmyjahh/AgencIA.git ~/AgencIA
bash ~/AgencIA/install.sh
```

> Requer **Git** e o **Claude Code**.

---

## O time

| Disciplina | Agente | O que faz |
|-----------|--------|-----------|
| 🎯 **orquestrador** | Orquestração | Diagnostica a demanda, roteia, sequencia a campanha e revisa a qualidade entre etapas |
| 📖 **branding** | Mensagem / posicionamento | Roteiro de marca, one-liner, clareza de oferta, esqueleto do funil |
| 🧠 **copy** | Copywriting | Níveis de consciência, headline, mecanismo, páginas de venda, VSL |
| 🎨 **design** | Criativo / visual | Prompts de IA, criativos de anúncio, identidade, thumbnails |
| 🚦 **trafego** | Tráfego pago | Meta Ads, públicos, orçamento, teste, escala, lançamento |

---

## Como usar

Ative o orquestrador e deixe ele conduzir:

```
@orquestrador
*campaign     # campanha completa (as 4 disciplinas em sequência)
*launch       # lançamento em ondas
*diagnose     # só rotear a sua demanda para o especialista certo
```

Ou vá direto a um especialista: `@branding`, `@copy`, `@design`, `@trafego`.

---

## Workflows pré-definidos

A campanha atravessa as 4 disciplinas automaticamente, com **portão de qualidade** entre cada etapa (input ruim a montante é barrado antes de desperdiçar verba a jusante):

| Comando | Workflow | Fluxo |
|---------|----------|-------|
| `*campaign` | **Campanha Completa** | `diagnose → branding → copy → design → trafego → review` |
| `*launch` | **Lançamento** | Campanha em ondas: pré-lançamento → aquecimento → abertura → escassez |

---

## Estrutura

```
AgencIA/
├── install.sh                  # instalador
├── squad.yaml                  # manifesto
├── config/config.yaml          # tiers, agentes, handoffs
├── data/routing-catalog.yaml   # mapa demanda → especialista
├── agents/                     # orquestrador + branding + copy + design + trafego
├── tasks/                      # diagnose, build-message, write-copy, create-creatives, build-traffic, review
├── workflows/                  # wf-full-campaign, wf-launch
└── checklists/output-quality.md
```

---

*AgencIA v1.0.0 · Agência de marketing em agentes de IA · MIT*
