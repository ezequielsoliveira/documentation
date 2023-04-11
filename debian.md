# Atenção

> Tecnologias podem ser atualizadas, verifique se há comandos mais recentes.
> Entenda os conceitos de funcionamento, comandos prontos podem ser um início.

# Comandos para verificar a versão do sistema operacional no debian:
- ```cat /etc/*-release```
- ```cat /proc/version```
- ```lsb_release -a```

# Comando para atualizar todo sistema operacional no debian:
- ```apt update -y && apt upgrade -y && apt dist-upgrade -y```

# Visualiza portas que aplicações estão escutando.
- ```netstat -tulpan```

# Logar como usuário root
- ```sudo su```

# Adicionar usuário ao grupo sudo
- ```usermod -a -G sudo {USERNAME}```

# Forma segura de editar o arquivo /etc/sudoers
- ```sudo visudo```

# Exibe as conexões de rede ativas que estão usando a porta 80
- ```netstat -tulpn | grep :80```

# Listar usuários
- ```cat /etc/passwd```

# Listar grupos
- ```getent group```

# Outros Comandos (necessário revisão)
- Alterar permissões de determinado caminho
  - ```chmod -R 770 {FULL_PATH}```
- Alterar proprietário e grupo de determinado caminho
  - ```chown -R {OWNER}:{GROUP} {FULL_PATH}```
- Definir GID
  - ```chmod -R g+s {FULL_PATH}```
- umask system file
  - ```cat /etc/login.defs```
- umask user file
  - ```~/.profile```
- umask use
  - ```umask 077```

# Ajeitar (apresentação de permissões de usuários no linux)

-rwxrwxrwx

"-" => arquivo
"d" => directory
"i" => link

"+" => adiciona permissão
"-" => remove permissão
"=" => substitui permissão

r => leitura
w => escrita
x => execução

"a" => all
"u" => user
"g" => group
"o" => other

-     rwx     rwx    rwx
file  user   group   other