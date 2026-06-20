# Guia Técnico-Metodológico — Site GitHub Pages

Este repositório contém duas versões do guia:

1. **`docs/`** — site HTML pronto para publicar no GitHub Pages usando **Deploy from a branch → main /docs**.
2. **`mkdocs-src/`** — projeto-fonte em MkDocs para edição futura.

## Publicação recomendada pelo GitHub Web

1. Crie um repositório no GitHub.
2. Envie todos os arquivos deste pacote para a branch `main`.
3. Vá em **Settings → Pages**.
4. Escolha **Deploy from a branch**.
5. Selecione **Branch: main** e **Folder: /docs**.
6. Salve.

Não é necessário criar branch `gh-pages`. O erro anterior ocorreu porque o pacote dependia de GitHub Actions/MkDocs; esta versão já inclui o HTML pronto.

## Edição avançada com MkDocs

Para editar e gerar novamente o site via MkDocs, use a pasta `mkdocs-src/`.
