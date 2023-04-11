# Atenção

> Tecnologias podem ser atualizadas, verifique se há comandos mais recentes.
> Entenda os conceitos de funcionamento, comandos prontos podem ser um início.

```echo "Parâmetros digitados: $1 $2 $3"```

```echo "A mensagem é: $mensagem"```

```A sintaxe $() é usada para substituir o resultado de um comando dentro de uma string, e não para acessar os parâmetros de uma função ou script shell. Para acessar o primeiro parâmetro de um script shell, você deve usar a sintaxe ${1} ou ${1:-default_value} (para fornecer um valor padrão caso o parâmetro não seja definido). Ou seja, A sintaxe $($1) está incorreta. Quando usamos $() estamos executando um comando dentro de uma string e substituindo a string pelo resultado do comando.```
