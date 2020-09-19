# Go Barber API

## :horse_racing: Iniciar a aplicação:

- O primeiro passo é iniciar os containers do docker referentes ao banco de dados PostgreSQL. Para isso basta executar no terminal `docker run --name gobarber-pg -e POSTGRES_PASSWORD=docker -p 5433:5432 -d postgres `.

- Após, levantar o container, crie um banco com o nome `gobarber`. Após isso, execute os seguintes comandos:

  - Executar `yarn` para instalar a dependências;

  - Executar `yarn typeorm migration:run` para rodar as migrations;

  - Executar `yarn dev:server` para levantar o servidor.
