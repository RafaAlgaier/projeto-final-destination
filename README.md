# 🌍 Final Destination

Aplicação web para planejamento de viagens, permitindo buscar destinos, consultar clima e gerenciar viagens de forma simples e intuitiva.

---

## 📌 Funcionalidades

* 🔐 Login de usuário
* 🔎 Busca de destinos
* 🌦 Consulta de clima em tempo real
* ✈️ Cadastro de viagens
* 📋 Listagem, edição e exclusão de viagens
* ⭐ Favoritar destinos
* 🌙 Modo dark

---

## 🛠 Tecnologias utilizadas


- **Framework CSS:** Bootstrap v5.3.3  
  *Escolhido por sua ampla documentação, responsividade pronta para mobile, tablet e desktop, além de componentes prontos como cards, modais e navbars, que facilitam a implementação do layout prototipado.*

- **JavaScript (ES6+) & jQuery v3.7.1**  
  *Para interatividade, manipulação do DOM e validação de formulários.*

- **Fake API:** JSON Server v0.17.x  
  *Permite simular um backend para persistência de dados de usuários e viagens.*

- **Web Storage (localStorage)**  
  *Para armazenar usuário logado, preferências e destinos favoritos localmente.*

- **API Pública:** OpenWeather API v2.5  
  *Integração para fornecer dados de clima em tempo real dos destinos pesquisados, enriquecendo a experiência do usuário com informações úteis e confiáveis.*

## Protótipo e Layout

O layout foi desenhado com base em **Bootstrap**, garantindo responsividade e consistência visual em todos os dispositivos. Cards de destinos, formulários de cadastro e login, e modais foram implementados usando componentes prontos do framework.

---

## ⚙️ Como executar o projeto

1. Instale as dependências (se necessário):

```
npm install
```

2. Inicie o servidor:

```
npx json-server --watch db.json --port 3000
```

3. Abra o arquivo:

```
login.html
```

no navegador.

---

## 📄 Documentação

Para mais detalhes sobre o projeto:

* 📘 [PRD (Product Requirements Document)](docs/prd.md)
* 📗 [Especificação Técnica (SPEC)](docs/spec.md)

---
## ✅ Checklist da Atividade

- [x] Clonei o repositório
- [x] Inicializei o Node.js (npm init)
- [x] Criei o arquivo .gitignore
- [x] Instalei dependências (jquery)
- [x] Instalei dependências de desenvolvimento (gh-pages)
- [x] Realizei commits e push no GitHub

## 👨‍💻 Autor

Projeto desenvolvido por **Rafa Algaier Teixeira** 🚀
