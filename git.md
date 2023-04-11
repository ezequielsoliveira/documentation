# Atenção

> Tecnologias podem ser atualizadas, verifique se há comandos mais recentes.
> Entenda os conceitos de funcionamento, comandos prontos podem ser um início.

# GIT no terminal (windows)

# Multiplas linhas na mensagem do commit.
- ```
  git commit -m "this is
  > a line
  > with new lines
  > maybe"
  ```

## Comando perigosos

- Excluir uma branch;
  - ```git branch --delete {BRANCH_NAME}```
- Mudar para uma branch que existe somente no repositório remoto (vai trazer ela para o local);
  - ```git checkout -b {BRANCH_NAME} origin/{BRANCH_NAME}```
- Restaurar o repositório a partir de um commit específico;
  - ```git reset --hard {COMMIT_HASH}```
  - ```git reset --soft "HEAD@{1}"```
  - ```commit -m {COMMIT_HASH}```
