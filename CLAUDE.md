# CLAUDE.md — Inventário E-commerce · Vulcabras

Regras gerais de trabalho: `C:\Repositórios\CLAUDE.md`. Resumo: plano + modelo antes de editar, PT-BR, economia de créditos, aprovado vai direto para `main`.

- `index.html` (dashboard) e `gerador.html`. HTML estático, sem build. Leia por trechos.
- Supabase `juoibcncsehzdelkhcnk`. Deploy Vercel a partir de `main`.
- É a referência do botão de tema: **"🌙 Tema Escuro" / "☀️ Tema Claro"** (spans `toggleIcon`/`toggleLabel` dentro de `btnTema`).
- Topbar padrão: perfil + Tela cheia + Tema + Sair.
- O ciclo de inventário e a meta do Inventário também aparecem no Abastecimento do Produtividade (`config_geral.ciclo_inventario_ativo`).
- **Identidade visual (padrão Vulcabras, desde 20/11/2026):** segue `docs/padrao-vulcabras/README.md` do repositório Produtividade---E-commerce, igual aos outros reports. Tokens `--bg`, `--bg-card`, `--border`, `--text`, `--text-muted`, `--accent`, `--olive`, `--amber`, `--red`, `--laranja`, `--gelo`; atributo `data-tema="escuro|claro"` (escuro é o padrão; a escolha fica em `localStorage` `inventario_tema`, compartilhada entre `index.html` e `gerador.html`). Nenhuma cor fixa fora do bloco de tokens no topo do CSS.
- **Única exceção ao padrão:** a navegação por telas fica em **abas no topo** (e não na barra lateral). Perfil (e-mail do login, lido do token) + Tela cheia + Tema + Sair continuam na topbar.
- Cards KPI: barra de 4 px com a cor do significado (`k-accent`, `k-olive`, `k-amber`, `k-laranja`, `k-red`). **Dourado (`--amber`) = a cor do inventário: itens contados** (barras do gráfico, arco do donut, barra do card), por decisão de 20/11; pendentes = `--laranja`; acuracidade = `--olive` (abaixo da meta `META_ACURACIDADE_PCT`, `--amber`).
- Logos: `img/logo-mark.png` (escuro) e `img/logo-mark-azul.png` (claro), trocadas por CSS (`.so-escuro`/`.so-claro`); ícone da aba `img/logo-mark.png` (o V colorido, igual aos outros reports; `img/favicon.png` só como `apple-touch-icon`). Nada de imagem em base64 no HTML.
- Linha de total de tabela: sempre `tr.total` (nunca `:last-child`). Colunas numéricas: classe `num` (alinhadas à direita).
