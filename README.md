# Inventário — Dashboard

Dashboard de inventário do CD, no padrão visual e de arquitetura do time.

> **Padrão visual da empresa:** cores, logos, componentes HTML, estrutura de
> projeto e padrão de apresentações estão em [`PADRAO-VULCABRAS.md`](PADRAO-VULCABRAS.md)
> — documento único, idêntico nos três repositórios do time.

## Arquivos

| Arquivo | O que é |
|---|---|
| `index.html` | O dashboard. Single-file: HTML + CSS + JS embutidos, sem build step. |
| `gerador.html` | Ferramenta auxiliar de geração. |
| `PADRAO-VULCABRAS.md` | Manual de identidade visual e padrões de projeto. |

## Antes de alterar qualquer coisa aqui

1. Leia o capítulo 8 do `PADRAO-VULCABRAS.md` — a separação entre cálculo e
   renderização não é opcional.
2. Mudança visual passa por mockup aprovado antes de ir para o arquivo de
   produção.
3. Rode o checklist do capítulo 11 antes de publicar.

## Projetos irmãos

- **report-ecommerce** — operação do CD de e-commerce (Outbound, Inbound,
  Estoque, Reversa, Balanço WMS×SAP).
- **report-DISTR** — balanço e detalhamento de estoque da distribuidora.
