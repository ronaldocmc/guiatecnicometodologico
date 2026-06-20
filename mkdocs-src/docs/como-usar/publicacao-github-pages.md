# Publicação no GitHub Pages

Este projeto já contém uma configuração básica para publicação com GitHub Actions.

## Passos

1. Crie um repositório no GitHub.
2. Envie os arquivos do projeto.
3. No GitHub, acesse **Settings → Pages**.
4. Em **Build and deployment**, selecione **GitHub Actions**.
5. Faça um commit na branch `main` ou `master`.
6. Aguarde o workflow finalizar.

## Execução local

```bash
pip install -r requirements.txt
mkdocs serve
```

## Geração estática

```bash
mkdocs build
```

O HTML será gerado na pasta `site/`.
