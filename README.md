# Baozi Store — API REST

Projeto da Atividade Prática de Desenvolvimento Web Back-End.

## Tecnologias
- Java 17
- Spring Boot 3.5.5
- Spring Web
- Spring Data JPA
- H2 (banco relacional em memória)
- JSON
- Postman

## Como executar
1. Instale Java 17+ e Maven.
2. No terminal, entre na pasta do projeto.
3. Execute `mvn spring-boot:run`.
4. A API ficará disponível em `http://localhost:8080`.

## Endpoints
### Clientes
- POST `/clientes`
- GET `/clientes`
- GET `/clientes/{id}`
- DELETE `/clientes/{id}`

### Produtos
- POST `/produtos`
- GET `/produtos`
- GET `/produtos/{id}`
- DELETE `/produtos/{id}`

### Pedidos
- POST `/pedidos`
- GET `/pedidos`
- GET `/pedidos/{id}`
- DELETE `/pedidos/{id}`

## Exemplos de JSON
### Cliente
```json
{
  "nome": "SEU NOME + RU",
  "clienteDesde": "2026-08-20"
}
```

### Produto
```json
{
  "nome": "Baozi Tradicional",
  "preco": 8.50,
  "estoque": true
}
```

### Pedido
```json
{
  "clienteId": 1,
  "produtoId": 1,
  "quantidade": 3
}
```
