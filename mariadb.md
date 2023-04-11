# Atenção

> Tecnologias podem ser atualizadas, verifique se há comandos mais recentes.
> Entenda os conceitos de funcionamento, comandos prontos podem ser um início.

# Executar comandos no MariaDB a partir de um arquivo SQL

mysql> source C:\LocalServer\nginx\html\Application\database.sql

# Solução de problemas

## Iniciar o banco de dados

- ```mysql_install_db```

> Conceito: quando o MySQL é instalado pela primeira vez, o comando "mysql_install_db" deve ser executado antes que o servidor MySQL possa ser iniciado. Esse é usado para inicializar o banco de dados MySQL e criar a estrutura básica de diretórios, arquivos e tabelas necessários para armazenar e gerenciar dados no MySQL Esse comando cria o diretório "data" padrão do MySQL, que contém os arquivos de banco de dados e configurações do servidor.

# Possíveis poluções de problemas

- Verifique se a senha do usuário está correta;
- Verifique se a conexão é autenticada por meio de senha ou socket;
- Se a conexão for estabelecida por senha, e for possível acessar o SGBD diretamente pela linha de comando, mas não pela aplicação, pode ser que a senha do usuário esteja inválida, altere a senha do usuário e tente novamente.
