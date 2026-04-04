# Especificação Técnica

## Tecnologias e Versões

- HTML5
- CSS3
- Bootstrap v5.3.3
- JavaScript (ES6+)
- jQuery v3.7.1
- JSON Server v0.17.x
- Web Storage (localStorage)
- OpenWeather API v2.5

---

# Modelo de Dados

O sistema possui duas principais entidades:

* Usuários
* Viagens

Usuários podem cadastrar múltiplas viagens.

---

# Diagrama de Dados (Mermaid)

```mermaid
erDiagram

USUARIO {
int id
string email
string senha
}

VIAGEM {
int id
string destino
date data
number orcamento
string tipo
}

USUARIO ||--o{ VIAGEM : cadastra
```

---

# Estrutura da Fake API

Exemplo do arquivo `db.json`.

```json
{
  "usuarios": [
    {
      "id": 1,
      "email": "usuario@email.com",
      "senha": "123456"
    }
  ],
  "viagens": [
    {
      "id": 1,
      "destino": "Paris",
      "data": "2026-07-10",
      "orcamento": 3000,
      "tipo": "lazer"
    }
  ]
}
```

---

## Integração com API Pública – OpenWeather

A aplicação utiliza a API OpenWeather para mostrar informações meteorológicas do destino pesquisado, como:

- temperatura (°C)
- descrição do clima
- ícone meteorológico

### Endpoint base
https://api.openweathermap.org/data/2.5/weather

### Exemplo de requisição com fetch

fetch(`https://api.openweathermap.org/data/2.5/weather?q=Paris&appid=API_KEY&units=metric`)
.then(response => response.json())
.then(data => console.log(data));

### Observações
- `API_KEY` deve ser substituída pela chave de acesso obtida no OpenWeather.
- Unidade de temperatura configurada em Celsius (`units=metric`).
---

# Persistência de dados

Os dados são armazenados de duas formas:

**JSON Server**

* armazenamento das entidades do sistema
* usuários
* viagens

**Web Storage**

* usuário logado
* preferências de tema
* destinos favoritos

---

# Arquitetura da aplicação

A aplicação segue uma organização simples baseada em separação de responsabilidades.

```
/docs
prd.md
spec.md

/css
style.css

/js
login.js
cadastro.js
viagens.js
api.js

index.html
login.html
cadastro.html
viagens.html
```

---

# Requisições assíncronas

A aplicação utiliza **fetch API** para comunicação com o JSON Server.

Exemplo:

```javascript
fetch("http://localhost:3000/viagens")
.then(response => response.json())
.then(data => console.log(data))
```

---

# Responsividade

O layout utiliza o Bootstrap Grid System e classes utilitárias (ex: col-md-6, mt-3, bg-primary) para adaptação a diferentes tamanhos de tela:

* Mobile
* Tablet
* Desktop
