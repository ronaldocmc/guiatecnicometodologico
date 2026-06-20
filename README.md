# Guia Técnico-Metodológico — Site MkDocs

Projeto completo em formato Git/MkDocs para publicar o Guia Técnico-Metodológico como site HTML no GitHub Pages.

## Como executar localmente

```bash
python -m venv .venv
source .venv/bin/activate  # Linux/macOS
# .venv\Scripts\activate  # Windows
pip install -r requirements.txt
mkdocs serve
```

Acesse: http://127.0.0.1:8000

## Como publicar no GitHub Pages

1. Crie um repositório no GitHub.
2. Envie todos os arquivos deste projeto.
3. Ative GitHub Pages via GitHub Actions.
4. O workflow `.github/workflows/deploy.yml` fará o build e publicará o site.

## Estrutura

- `docs/`: páginas do site.
- `docs/tipos/`: tipos de proposta.
- `docs/conceitos/`: conceitos fundamentais.
- `docs/fundamentos/`: fundamentação teórica e metodológica.
- `docs/artefatos/`: artefatos, metadados e contratos.
- `docs/metricas/`: métricas e avaliação.
- `docs/tecnicas/`: técnicas, métodos e ferramentas.
- `docs/problemas/`: problemas e lacunas.
- `docs/aplicacoes/`: aplicações por domínio.
- `docs/trilhas/`: roteiros de estudo.
- `docs/templates/`: modelos reutilizáveis.
