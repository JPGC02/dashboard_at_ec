# Dashboard AT - Engenharia Clinica | Medsystem

Dashboard de Assistencia Tecnica de Equipamentos de Engenharia Clinica.

## Hospedagem

- **Repo GitHub:** [JPGC02/dashboard_at_ec](https://github.com/JPGC02/dashboard_at_ec)
- **Deploy:** Netlify (auto-deploy via push na branch `main`)

## Estrutura

```
.
├── index.html          # Arquivo servido pelo Netlify na raiz
├── at_dashboard.html   # Copia com nome original (opcional, mesmo conteudo)
├── netlify.toml        # Configuracao de build/deploy do Netlify
└── README.md
```

## Fluxo de atualizacao

1. Cron (a definir) coleta dados da fonte (Supabase / planilha / etc).
2. Atualiza `index.html` localmente.
3. Faz `git commit` + `git push` para `main`.
4. Netlify detecta o push e faz deploy automatico.

## Atualizacao manual

```bash
git pull
# editar/regerar index.html
git add index.html
git commit -m "chore: atualiza dashboard"
git push
```
