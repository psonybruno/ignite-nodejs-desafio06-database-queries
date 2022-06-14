# [NODEJS] Desafio 06: Database Queries

## Ambiente para os testes
```
docker run --name ignite-challenge-database-queries -e POSTGRES_DB=queries_challenge -e POSTGRES_PASSWORD=docker -p 5432:5432 -d postgres
docker stop ignite-challenge-database-queries
docker start ignite-challenge-database-queries
```
### Database
- [ ] Criar banco de dados no *Postgres* como o nome **queries_challenge**;
- [ ] Alterar os dados no **ormconfig.json**;

## Repositórios da aplicação
### UsersRepository
- Método **findUserWithGamesById**;
- Método **findAllUsersOrderedByFirstName**;
- Método **findUserByFullName**;

### GamesRepository
- Método **findByTitleContaining**;
- Método **countAllGames**;
- Método **findUsersByGameId**;

## Específicação dos testes
### Requisitos
#### UsersRepository
- [x] should be able to find user with games list by user's ID;
- [x] should be able to list users ordered by first name;
- [x] should be able to find user by full name;

#### GamesRepository
- [x] should be able find a game by entire or partial given title;
- [x] should be able to get the total count of games;
- [x] should be able to list users who have given game id;
