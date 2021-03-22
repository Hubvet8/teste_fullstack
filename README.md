# Teste para Desenvolvedor Fullstack

Esse é um teste prático (Hard Skills) para conhecermos melhor suas habilidades e entender como você desenvolve seus projetos. 
Mostre todo seu potencial 😎. Boa sorte! Esperamos você do outro lado.

Quando finalizar o teste, publique em um repositório seu no [Github](https://github.com) ou [Gitlab](https://gitlab.com) e envie um email com o título `[Teste Fullstack] Seu nome` para **ti@hubvet.cloud**

## Backend

Desenvolver uma **API RESTful** em **[(PHP) Laravel/Lumen](https://lumen.laravel.com/)** - ou - **[(Node.js) Express](https://expressjs.com/pt-br/)** que utilize todos os métodos (`GET`, `POST`, `PUT`, `PATCH`, `DELETE`).  

### Especificação

Monte uma base de veículo com a seguinte estrutura:

```
--- Tabela: marcas ---
id:           integer (auto increments)
nome:         string

--- Tabela: veiculos ---
id            integer (auto increments)
veiculo:      string
marca_id:     integer (referência "id" em "marcas")
ano:          integer
descricao:    text
vendido:      bool
created_at:   datetime
updated_at:   datetime
```

Utilize **MySQL** ou **MongoDB** para armazenar os dados que a **API** irá consumir.

### Bônus (Like a boss) 😎
Não pedimos isso no teste, mas se fizer será visto com bons olhos

- Autenticação com JWT
- Teste Unitário da API (HTTP Test)
- Container Docker
- Implementar Cache com Redis
- Design Patterns (SOLID, Service Container)


### API endpoints

`GET /veiculos`

Retorna todos os veículos (com detalhes da Marca)

---

`GET /veiculos/{id}`

Retorna os detalhes do veículo (com detalhes da Marca)

---

`POST /veiculos`

Adiciona um novo veículo

---

`PUT /veiculos/{id}`

Atualiza os dados de um veículo

---

`PATCH /veiculos/{id}`

Atualiza apenas o status de "vendido" para `true` ou `false`

---

`DELETE /veiculos/{id}`

Excluir o veículo


## Frontend

Desenvolver uma **Aplicação SPA** em **[Vue.js](https://vuejs.org/)** - ou - **[Angular](https://angular.io/)** de acordo com o desenho que está na pasta `/layout`

### Especificação

- Consumir **API** criada acima
- Criar uma tela que tenha...
    - Listagem de veículos
    - Detalhe do veículo
    - Busca
    - Formulário de cadastro/edição de veículos

### Dica

Utilize algum framework para auxiliar no desenvolvimento da interface, por exemplo:

- https://vuetifyjs.com/
- https://getbootstrap.com/
- https://materializecss.com/

## Dúvida

Se tiver qualquer dúvida sobre esse teste, envie um email com o título `[Teste Fullstack] O assunto que vc deseja` para ti@hubvet.cloud
