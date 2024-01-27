<h1>Projeto DSList - Intensivão Java Spring</h1>

 ![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
 ![Spring](https://img.shields.io/badge/Spring-6DB33F.svg?style=for-the-badge&logo=Spring&logoColor=white)
 ![Postgres](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

 <p>Projeto foi desenvolvido durante o curso Intensivão Java Spring oferecida pela <a href="https://devsuperior.com.br/">DevSuperior.</a> O projeto consiste em uma 
   Api Rest de Gerenciamento de Entregas</p>

   <h2>Sumário</h2>
  <ul>
    <li><a href="#tecnologia">Tecnologias</li>
    <li><a href="#praticas">Diagrama de Classes</li>
    <li><a href="#api">Documentação API</li>
</ul>

<h2 id="tecnologia">Tecnologias</h2>
<p>Spring Boot | Spring MVC | Spring Data JPA | PostgreSQL | Docker</p>

<h2 id="praticas">Diagrama de Classes</h2>

 <img src="https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/dslist-model.png">

 <h2 id="api">Documentação API</h2>
<h4>URL base</h4>

     http://localhost:8080/dslist/
     
<h4>Obter Listagem dos Games Cadastrados</h4>

     GET /games

<h4>Buscar Listagem dos Games Cadastrados Pelo Id</h4>

    GET /games/{id}
    
| Parâmetro | Tipo  | Descrição                    |
|-----------|-------|------------------------------|
| id        | Long  | Obrigatório. Id do Game      |

<h4>Obter Listagem das Listas de Games Cadastrados</h4>

    GET /lists

<h4>Buscar Listagem das Listas de Games Cadastrados Pelo Id da Lista</h4>

    GET /lists/{id}/games

| Parâmetro | Tipo  | Descrição                        |
|-----------|-------|----------------------------------|
| id        | Long  | Obrigatório. Id da Lista de Game |

<h4>Mudar a posição do Game dentro de uma Lista de Game</h4>

    POST /lists/{id}/replacement

| Parâmetro | Tipo            | Descrição                                       |
|-----------|-----------------|-------------------------------------------------|
| id        | Long            | Obrigatório. Id da Lista de Game               |
| body      | ReplacementDTO  | Obrigatório. Informações da posição de origem e posição destino |






 
