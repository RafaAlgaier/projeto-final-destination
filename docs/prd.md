# Product Requirements Document (PRD)

## Identificação

**Aluno:** Rafael Algaier
**Projeto:** Final Destination
**Disciplina:** Desenvolvimento Web

---

# Descrição do Sistema 

O **Final Destination** é uma aplicação web responsiva inspirada em plataformas de hospedagem e planejamento de viagens como Airbnb e Booking.com.

O objetivo do sistema é permitir que usuários pesquisem destinos, consultem informações sobre cidades (como clima) e cadastrem suas próprias viagens para organizar seus planos.

O sistema resolve o problema de **organização de viagens**, permitindo que o usuário registre destinos, datas e orçamento em um único lugar.

---
## ⚙️ Regras de Negócio

- O usuário deve estar autenticado para cadastrar, editar ou excluir viagens.
- Cada viagem deve conter destino, data e orçamento obrigatoriamente.
- A consulta de clima será feita em tempo real através de uma API externa.
- Um usuário pode ter múltiplas viagens cadastradas.
- Apenas o usuário dono da viagem pode editá-la ou excluí-la.
- O sistema deve ser responsivo (mobile e desktop).

# Histórias de Usuário

## Autenticação

**US01**

Como visitante, eu quero fazer login no sistema para acessar minhas viagens cadastradas.

---

## Buscar destinos

**US02**

Como visitante, eu quero pesquisar um destino para visualizar informações e planejar uma viagem.

---

## Consultar clima

**US03**

Como visitante, eu quero consultar o clima de uma cidade para decidir quando viajar.

---

## Cadastro de viagem

**US04**

Como usuário autenticado, eu quero cadastrar uma viagem informando destino, data e orçamento para organizar meus planos.

---

## Listagem de viagens

**US05**

Como usuário autenticado, eu quero visualizar minhas viagens cadastradas para acompanhar meus planos.

---

## Editar viagem

**US06**

Como usuário autenticado, eu quero editar informações de uma viagem para atualizar dados incorretos.

---

## Excluir viagem

**US07**

Como usuário autenticado, eu quero excluir uma viagem cadastrada para remover planos que não são mais necessários.

---

## Favoritar destinos

**US08**

Como usuário autenticado, eu quero favoritar destinos para salvar lugares que desejo visitar futuramente.

---

## Preferência de tema

**US09**

Como usuário, eu quero ativar o modo escuro para melhorar a visualização do site à noite.

---

## Responsividade

**US10**

Como usuário, eu quero acessar o sistema pelo celular ou computador para planejar viagens em qualquer dispositivo.
