# DSlist

https://dslist-production-44bb.up.railway.app

DSList é uma aplicação backend com listagem de games por categoria.
O usuário poderá reordenar a posição do game de acordo com o desejado.

Desenvolvida durante as aulas do Intensivão Java Spring da DevSuperior.

## Tecnologias utilizadas
- Java
- Spring Boot
- Postgress

## Screenshots:
- Modelo de Dominio
> <img src="README/Modelo Dominio.png" style="width:700px;"/>

- GET Games
> <img src="README/Games.png" style="width:500px;"/>

- GET Listas de Categorias
> <img src="README/Lists.png" style="width:500px;"/><br/>

- GET Game por Id
> <img src="README/Games by id.png" style="width:500px;"/>

- GET games por lista categoria
> <img src="README/Games by lists.png" style="width:500px;"/>

- POST reordenação de games
> <img src="README/Lists replacement.png" style="width:500px;"/>

## Executando o projeto localmente

### Pré-requisitos
- JDK 17 instalado e variáveis de ambiente configuradas.
- Git instalado.
- Eclipse (ou outra IDE de sua preferência) instalado
- Docker instalado (apenas para o ambiente de desenvolvimento com PostgreSQL)

### Passos

- Clone o repositório do DSList: git clone https://github.com/jsidegum/dslist
- Abra o Eclipse (ou sua IDE) e importe o projeto Maven existente.
- Instale o plug-in "Spring Tools 4" no Eclipse e reinicie, se necessário
- Configure o JRE instalado para utilizar o JDK 17.
- Para o ambiente de teste com H2:
  - Execute o projeto em "Run As > Spring Boot App".
  - Acesse a rota de teste: http://localhost:8080/games
  - Acesse o banco de dados: http://localhost:8080/h2-console
- Para o ambiente de desenvolvimento com PostgreSQL (usando Docker):
  - No arquivo "application.properties", altere "test" para "dev".
  - No arquivo "application-dev.properties", descomente os comentários.
  - Inicie o contêiner "docker-dslist" que deve estar previamente configurado.
  - Execute o projeto em "Run As > Spring Boot App".
  - Acesse a rota de teste: http://localhost:8080/games
  - Acesse o banco de dados: http://localhost:5050
