# Projeto CRUD de Regiões

Esta é uma API de **cadastro e gerenciamento de regiões**, desenvolvido em c#.net com arquitetura simplificada para ser consumida por um frontend independente.

O sistema permite a **criação, listagem, edição, ativação e inativação** de regiões, respeitando regras como unicidade por UF + Nome e controle de status.

Este projeto tem como objetivo ser um backend base para uma avaliação de desenvolvimento de um frontend em vue.js.

---

## Como executar o projeto?

### Pré-Requisitos de Ferramentas Instaladas
- ✔️ Visual Studio Comunity (VSC)
- ✔️ PostgreSQL

### Preparação do Banco de Dados
- ✔️ No VSC, abra o arquivo appsettings.json e ajuste em "ConnectionStrings > DefaultConnection" o usuário e senha para acesso ao BD.
- ✔️ No VSC, no "Console Gerenciador de Pacotes", Selecione o projeto "RegionAPI" e execute o comando "Update-Database", para criar o banco de dados.

### Executar a API
- ✔️ Agora basta apertar a tecla F5 no VSC para executar o projeto e levantar a API.
- ✔️ Provalmente ela irá rodar no endereço https://localhost:7278. Confirme olhando o endereço que será aberto automaticamente no navegador após ter pressionado o F5.
- ✔️ Use este endereço na sua aplicação frontend.

---

## Tecnologias Utilizadas

### **Backend** (.NET + PostgreSQL)
- ASP.NET Core Web API (C#)
- Entity Framework Core com Code First
- PostgreSQL com migrations
- LINQ para consultas ordenadas e validações
- Injeção de dependência (`RegionService`)
- ViewModels e DTOs
- Configuração de CORS para frontend React

### **Testes**
- xUnit com cobertura da `RegionService`
- Banco de dados InMemory para isolamento
- Validação de criação, duplicação, edição, ativação e ordenação

---

## Banco de dados utilizado POSTGRESQL.
- Foi utilizado o banco de dados POSTGRESQL para a realização de manipulação dos dados vigentes.
