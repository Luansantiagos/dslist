Este é o README para documentar a API REST que faz parte do meu portfólio. A aplicação é focada apenas no back-end e
foi desenvolvida utilizando Java na semana Intensivão Java Spring DevSuperior (Nélio Alves)

A API é uma aplicação back-end que oferece endpoints para gerenciar as requisições HTTP do front-end que retornam uma lista de jogos, um jogo específico de acordo
com o seu ID e define uma ordem na lista. Aplicação rodando em container via docker com configuração de esteira CI/CD na nuvem utilizando a plataforma Railway.

Tecnologias Utilizadas

Java 17

Spring Boot 3.1.1

H2 Database

Postgresql

Maven

Hibernate

Spring Initializer

Postman

Docker

Railway

Instruções de Uso
Pré-requisitos: Certifique-se de ter o Java 17 instalado em sua máquina.
Clone este repositório para sua máquina local usando o seguinte comando:

git clone https://github.com/luansantiagos/dslist.git

Navegue até o diretório do projeto:

cd nome-do-repositorio

Execute o aplicativo usando o seguinte comando:

./mvnw spring-boot:run
ou se você tiver o Maven instalado globalmente:
mvn spring-boot:run

A aplicação estará disponível em http://localhost:8080 (ou em outra porta, se configurada de forma diferente).
Aplicação também disponível na nuvem nos endpoints abaixo:

Endpoints
A API fornece os seguintes endpoints:

GET https://dslist-production-dcc4.up.railway.app/games [Puxa a lista completa de games do banco de dados]
![image](https://github.com/Luansantiagos/dslist/assets/95258692/03be1a5f-4715-4682-83c2-a83861cf4b06)

GET https://dslist-production-dcc4.up.railway.app/games/2 [Retorna um game específico no banco de dados de acordo com o ID passado no endpoint]
![image](https://github.com/Luansantiagos/dslist/assets/95258692/7737e589-ab9c-44a6-9a93-fe072c2d126e)

GET https://dslist-production-dcc4.up.railway.app/lists [Retorna a sublista dos games]
![image](https://github.com/Luansantiagos/dslist/assets/95258692/3dbf157d-156d-43fb-a8d6-7b9662fc9760)

GET https://dslist-production-dcc4.up.railway.app/lists/2/games [Retorna um game específico de acordo com o seu ID, acrescentado de uma breve descrição e sublista.]
![image](https://github.com/Luansantiagos/dslist/assets/95258692/b85da051-f21e-413a-87ca-f14070065167)

POST http://dslist-production-dcc4.up.railway.app/lists/2/replacement [Atualiza a ordem dos jogos no banco de dados de acordo com as informações de fonte e destino passadas
no corpo da requisição JSON]
![image](https://github.com/Luansantiagos/dslist/assets/95258692/7a844c65-3110-4509-8783-efc52a56a19e)

Considerações Finais
Este projeto foi desenvolvido como parte do meu portfólio para demonstrar minhas habilidades e conhecimentos em desenvolvimento de APIs REST em Java.
Sinta-se à vontade para explorar o código e os endpoints disponíveis.

Caso você tenha alguma dúvida ou sugestão, fique à vontade para entrar em contato comigo. Você pode me encontrar em:

Luan Santiago
luansantiagos@gmail.com
https://www.linkedin.com/in/luan-santiago-72a027121/

Espero que você aprecie este projeto!








