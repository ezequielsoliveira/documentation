# Atenção

> Tecnologias podem ser atualizadas, verifique se há comandos mais recentes.
> Entenda os conceitos de funcionamento, comandos prontos podem ser um início.

# Comando gerais
- Máquinas virtuais rodando
  - ```docker ps```
- Máquinas virtuais que foram criadas
  - ```docker ps -a```
- Excluir contianer
  - ```docker rmi -f {IMAGE_NAME}```
- Excluir imagem
  - ```docker rm {IMAGE_NAME}```
- Executar imagem criada pelo id
  - ```docker run -i -t {CONTAINER_ID} /bin/bash```

