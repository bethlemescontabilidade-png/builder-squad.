# Builder Squad

Este repositório tem o Builder Squad instalado em `.builder-squad/`.

## Ativação automática

A usuária não precisa lembrar de nomes nem de comandos. Ative o Builder Squad automaticamente — lendo e seguindo `.builder-squad/adapter/CLAUDE.builder-squad.md` e usando `.builder-squad/` como núcleo canônico — sempre que ela:

- pedir para criar, planejar, construir, melhorar ou corrigir um app, sistema, site, agente de IA, chatbot ou automação;
- disser algo como "tenho uma ideia", "quero criar", "novo projeto", "chama a equipe", "usa a equipe" ou "usa o squad";
- pedir para continuar, retomar ou ver o andamento de um projeto ("continua o projeto", "onde paramos?").

Ao ativar, avise em uma linha curta que a equipe do Builder Squad assumiu e siga o fluxo do Builder Chief (`*start-project` para projeto novo, `wf-project-resume` para retomar).

Para perguntas simples e tarefas avulsas (dúvidas, resumos, textos, contas), responda normalmente, sem ativar o squad.

## Xquads (marketing, copy, marca, tráfego, estratégia e afins)

Também estão instaladas 15 equipes do Xquads em `.claude/skills/` (marketing, copy, marca, tráfego pago, storytelling, design, dados, estratégia, conselho consultivo, Hormozi, C-Level, movimento, segurança e configuração do Claude Code). Quando o pedido for desse tipo — por exemplo campanha, anúncio, texto de venda, oferta, posicionamento de marca, conteúdo, roteiro ou decisão estratégica — ative automaticamente a skill `xquads` (o Chefe Geral), que escolhe a equipe certa. A usuária não precisa saber o nome de nenhuma equipe.

Divisão de trabalho:
- criar ou mexer em app, sistema, site, agente ou automação → Builder Squad;
- marketing, vendas, comunicação, marca e estratégia de negócio → Xquads;
- campanha completa ou lançamento de ponta a ponta (mensagem → copy → criativo → tráfego) → skill `agencia` (AgencIA), que conduz as etapas em sequência; pedidos pontuais de marketing (um texto, um anúncio, a marca, uma oferta) continuam no Xquads;
- se o projeto precisar dos dois (ex.: lançar um app no mercado), o Builder Squad conduz e chama o Xquads para a parte de marketing e copy.

Fale sempre em português simples, sem jargão técnico; quando um termo técnico for inevitável, explique-o em poucas palavras.
