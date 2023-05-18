# Preparar ambiente

- Instale o JDK 17 e configure as variáveis de ambiente correspondentes.
- Clone o repositório <https://github.com/jsidegum/dslist>.
- Instale o Eclipse ou outra IDE de sua preferência.
- No Eclipse, instale o plug-in "Spring Tools 4" (é necessário reiniciar).
- Configure o JRE instalado para utilizar o JDK 17.
- Importe o projeto "dslist" como um projeto Maven existente.
 
## Executar em ambiente de teste (H2)

- Execute o projeto em "Run As > Spring Boot App".
- Teste a rota: <http://localhost:8080/games>
- Banco de dados: <http://localhost:8080/h2-console>

## Executar em ambiente de desenvolvimento (PostgreSQL com Docker)

- No arquivo "application.properties", altere "test" para "dev".
- No arquivo "application-dev.properties", descomentar todos os comentarios
- Inicie o contêiner "docker-dslist" que deve estar previamente configurado.
- Execute o projeto em "Run As > Spring Boot App".
- Teste a rota: <http://localhost:8080/games>
- Banco de dados: <http://localhost:5050>
