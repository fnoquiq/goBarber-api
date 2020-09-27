# Go Barber API

## :horse_racing: Iniciar a aplicação:

- O primeiro passo é iniciar os containers do docker referentes aos banco de dados. Para isso basta executar no terminal:

  - PostgreSQL: `docker run --name gobarber-pg -e POSTGRES_PASSWORD=docker -p 5433:5432 -d postgres`;

  - MongoDB: `docker run --name gobarber-mongo -p 27017:27017 -d -t mongo`;

  - Redis: `docker run --name gobarber-redis -p 6379:6379 -d -t redis:alpine`;

- Após, levantar o container, crie um banco com o nome `gobarber`. Após isso, execute os seguintes comandos:

  - Executar `yarn` para instalar a dependências;

  - Executar `yarn typeorm migration:run` para rodar as migrations;

- Por fim, execute `yarn dev:server` para levantar o servidor.
