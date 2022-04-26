# Projeto para Pessoa Desenvolvedora Java

## 🏗 O que fazer?

- Você deve criar um projeto no git ou enviar o código para o email: ruan.a.bessa@kroton.com.br (No caso, se for git, enviar o link)
- Poderá ser realizado em dupla ou individual
- Data final para entrega: ##/##/####
- Poderemos acrescentar mais requisitos no projeto, até o dia ##/##/####

# 🚨 Requisitos

- A API deve ser construída em Java (8 ou superior) utilizando Spring Framework (2.2 ou superior)
- Implementar operações no banco de dados utilizando ***Spring Data JPA*** & ***Hibernate***
- **Bancos relacionais permitidos**
    - *MySQL*
    - *PostgreSQL* (prioritariamente)
- As entidades deversão ser criadas como tabelas utilizando a ferramenta de migração **Flyway**. Portanto, os scripts de **migrations** para geração das tabelas devem ser enviados no teste
- Sua API deverá seguir os padrões REST na construção das rotas e retornos
- Sua API deverá conter documentação viva utilizando a *OpenAPI Specification* (**Swagger**), ou sua API deverá conter a collection/variáveis do postman
- Caso haja alguma particularidade de implementação, instruções para execução do projeto deverão ser enviadas

# 🎁 Extra

- Testes unitários (Pesquisar utilização, e documentar os testes também)

# 🕵🏻‍♂️ Itens a serem avaliados

- Estrutura do projeto
- Utilização de código limpo e princípios **SOLID**
- Boas práticas da Linguagem/Framework
- Migrations para a criação das tabelas do banco relacional
- Seu projeto deverá seguir tudo o que foi exigido na seção  [O que desenvolver?]

# 🖥 O que desenvolver?

Você deverá criar uma API que o site [IMDb](https://www.imdb.com/) irá consultar para exibir seu conteúdo, sua API deverá conter as seguintes funcionalidades:

- Administrador
    - Cadastro
    - Edição
    - Exclusão lógica (desativação)
    - Listagem de usuários não administradores ativos
        - Opção de trazer registros (Se conseguir pode trazer eles paginados)
        - Retornar usuários por ordem alfabética
- Usuário
    - Cadastro
    - Edição
    - Exclusão lógica (desativação)
- Filmes
    - Cadastro (somente um usuário administrador poderá realizar esse cadastro)
    - Voto (a contagem de votos será feita por usuário de 0-4 que indica quanto o usuário gostou do filme)
    - Listagem
        - Opção de filtros por diretor, nome, gênero e/ou atores
        - Opção de trazer registros (Se conseguir pode trazer eles paginados)
        - Retornar a lista ordenada por filmes mais votados e por ordem alfabética
    - Detalhes do filme trazendo todas as informações sobre o filme, inclusive a média dos votos

**Obs.:** 

**Apenas os usuários poderão votar nos filmes e a API deverá validar quem é o usuário que está acessando, ou seja, se é um usuário administrador ou não.**

**Caso não consiga concluir todos os itens propostos, é importante que me envie a implementação até onde foi possível para que possa avaliar**
