# Atenção

> Tecnologias podem ser atualizadas, verifique se há comandos mais recentes.
> Entenda os conceitos de funcionamento, comandos prontos podem ser um início.

## MySQL (instalado manualmente de forma insegura pelo ZIP no Windows)

- Gerar bases de dados padrão do MySQL na primeira inicialização (escolher uma forma, segura ou não);
  - ```mysqld --initialize```
  - ```mysqld --initialize-insecure --console```

- Iniciar MySQL;
  - ```mysqld --console```

- Executar comandos diretamente no SGBD (a senha padrão é em branco);
  - ```mysql -u root -p```

- Alterar senha do usuário root para root.
  - ```mysql -u root -p```
  - ```ALTER USER 'root'@'localhost' IDENTIFIED BY 'root';```
  - ```FLUSH PRIVILEGES;```

# Possíveis poluções de problemas

- Verifique se a senha do usuário está correta;
- Verifique se a conexão é autenticada por meio de senha ou socket;
- Se a conexão for estabelecida por senha, e for possível acessar o SGBD diretamente pela linha de comando, mas não pela aplicação, pode ser que a senha do usuário esteja inválida, altere a senha do usuário e tente novamente.
