# Atenção

> Tecnologias podem ser atualizadas, verifique se há comandos mais recentes.
> Entenda os conceitos de funcionamento, comandos prontos podem ser um início.

# Comando certbot para instalar somente certificado digital

- ```sudo certbot certonly --standalone --preferred-challenges http -d {DOMAIN_NAME}```

# Comando certbot para instalar o certificado digital com o Nginx

-```certbot --nginx```

# Comando certbot para renovar o certificado digital existente

- ```certbot renew```

# Possíveis locais de instalação padrão dos certificados
- ```/etc/letsencrypt/live/capedac.org/fullchain.pem```
- ```/etc/letsencrypt/live/capedac.org/privkey.pem```
