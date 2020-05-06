# Ambiente Docker teste com PHP 8-fpm, Composer, Nginx e MySQL 8

Para executar:

`git clone https://github.com/gilbertoalbino/php80-fpm-docker.git`

`cd php80-fpm-docker/docker`

`docker-compose up -d`

## Importante

Se as portas **80** e **3306** estiverem em uso, no arquivo `docker/docker-compose.yml` mude para algo como:

```
  nginx:
    ...
    ports:
      - "8080:80"
      - "4430:443"

  mysql:
    ...
    ports:
      - "33066:3306"
```

Ou para alguma outra combinação de portas abertas no seu sistema operacional.

Abra o navegador em **http://localhost** e pronto!

Você deverá ver a tela do `phpinfo()`.

Daí pra frente espero que você saiba o que fazer! :P
