# Convenção de Commits

É recomendado utilizar a convenção **Conventional Commits** na mensagem de commits.

A especificação **Conventional Commits** é uma convenção leve sobre as mensagens de confirmação. Ela fornece um conjunto fácil de regras para criar um histórico de confirmação explícito; o que facilita a escrita de ferramentas automatizadas.

https://www.conventionalcommits.org

A mensagem de confirmação deve ser estruturada da seguinte forma:

```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

Tipos recomendados:
```build:, chore:, ci:, docs:, feat:, fix:, perf:, refactor:, revert:, style:, test:```

Descrição dos Tipos:

- **build**: alterações que afetam o sistema de compilação ou dependências externas
- **ci**: alterações em nossos arquivos e scripts de configuração de CI
- **docs**: alteração na documentação
- **feat**: um novo recurso
- **fix**: uma correção de bug
- **perf**: uma mudança de código que melhora o desempenho
- **refactor**: uma alteração de código que não corrige um bug nem adiciona um recurso
- **style**: alterações que não afetam o significado do código (espaço em branco, formatação, falta de ponto-e-vírgula etc.)
- **test**: adicionando testes ausentes ou corrige testes existentes

## Exemplos de Commits

Mensagem de commit sem corpo
```docs: correct spelling of CHANGELOG```

Mensagem de commit com multiplos parágrafos no copor e rodapé
```
fix: prevent racing of requests

Introduce a request id and a reference to latest request. Dismiss
incoming responses other than from latest request.

Remove timeouts which were used to mitigate the racing issue but are
obsolete now.

Reviewed-by: Z
Refs: #123
```
