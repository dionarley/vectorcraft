# Fork da Forja — `forja`

Este é um fork de `storytold/vectorcraft` mantido pela plataforma **Forja**
(`dionarley/forja`). A branch `forja` é a mainline do fork: é o que o monorepo
fixa no submodule (`apps/vectorcraft`). Mudanças entram aqui, **sem PR na origem**.

## O que muda nesta branch

Nada por enquanto: a branch é o upstream na versão que a Forja usa. Cada mudança
entra aqui com o motivo, em uma linha.

## Atualizar a partir da origem

```sh
git remote add upstream https://github.com/storytold/vectorcraft.git   # uma vez
git fetch upstream
git checkout forja
git rebase upstream/main
git push --force-with-lease origin forja
```

Depois, no monorepo: `git add apps/vectorcraft && git commit -m "chore: atualiza vectorcraft"`.

