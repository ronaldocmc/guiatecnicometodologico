# Como publicar sem precisar criar branch extra

Este pacote já vem com o site HTML pronto dentro da pasta `docs/`.

## Passos no GitHub Web

1. Crie um repositório novo no GitHub.
2. Faça upload de **todos os arquivos e pastas deste pacote** para a branch `main`.
3. Entre em **Settings** → **Pages**.
4. Em **Build and deployment**, escolha **Deploy from a branch**.
5. Em **Branch**, selecione `main`.
6. Em **Folder**, selecione `/docs`.
7. Clique em **Save**.

Pronto: o GitHub Pages publicará os arquivos HTML estáticos.

## Observação importante

Um arquivo ZIP não cria branch automaticamente no GitHub. A branch `main` aparece depois que o primeiro upload é feito no repositório. Este pacote foi ajustado para funcionar com `main /docs`, sem exigir branch `gh-pages`.

## Fonte MkDocs

A pasta `mkdocs-src/` contém o projeto MkDocs original. Ela pode ser usada futuramente para editar o site com MkDocs, mas a publicação imediata pelo GitHub Pages deve usar a pasta `docs/`, que já contém o HTML pronto.
