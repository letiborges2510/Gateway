# API Gateway - Spring Boot

Este módulo é responsável por atuar como ponto de entrada único para os microsserviços do sistema, utilizando Spring Cloud Gateway.
O gateway centraliza as requisições e realiza o roteamento para os serviços de cliente, login e produto, facilitando a comunicação e organização da arquitetura.

---

## Objetivo

Implementar um gateway para gerenciar o acesso aos microsserviços, aplicando conceitos de:

* Arquitetura de microsserviços
* Roteamento de requisições
* Centralização de acesso
* Organização e desacoplamento entre serviços

---

## Tecnologias Utilizadas

* Java 17+
* Spring Boot
* Spring Cloud Gateway

---

## Estrutura do Projeto

```bash
src/main/java/com/example/gateway
│
└── GatewayApplication.java  # Classe principal

```

--- 

# Funcionamento

O Gateway recebe todas as requisições e as redireciona automaticamente para o serviço correspondente, com base na URL acessada.

Exemplo:

Requisições para /accounts são direcionadas para o serviço de login
Requisições para /cliente são direcionadas para o serviço de cliente
Requisições para /produtos e /venda são direcionadas para o serviço de produto

---
##  Gateway Cliente

<img width="928" height="767" alt="gateway-cliente" src="https://github.com/user-attachments/assets/191c5fbb-20ab-44ad-a3ad-8a47c6f633bd" />

---

##  Gateway Login

<img width="1107" height="782" alt="gateway-login-1" src="https://github.com/user-attachments/assets/d101fb99-41cd-4c4f-910e-a4624a81a374" />

---

<img width="1067" height="672" alt="gateway-login-2" src="https://github.com/user-attachments/assets/8797bdee-5e85-48bc-a59c-627f82e95422" />

---

##  Gateway Produtos

<img width="1107" height="871" alt="gateway-produtos" src="https://github.com/user-attachments/assets/5185f645-452c-4832-9b09-b120d60da2b9" />

---

##  Gateway Vendas

<img width="1080" height="751" alt="gateway-venda" src="https://github.com/user-attachments/assets/af899f5d-8187-44a8-983a-bcb59218be70" />

---

##  Autoras

Projeto desenvolvido por:

* **Yasmin Oliveira**
* **Letícia Borges**

---

## Contexto Acadêmico

Este projeto foi desenvolvido como **atividade avaliativa**, contemplando a construção de uma arquitetura baseada em microsserviços, dividida em diferentes módulos:

* 🧑‍💼 **Cliente** → gerenciamento de clientes
* 🔐 **Login** → autenticação de usuários
* 📦 **Produto** → controle de produtos
* 🌐 **Gateway** → centralização das requisições e roteamento entre serviços

---

## Arquitetura do Projeto

A aplicação segue o padrão de microsserviços, onde cada módulo possui sua responsabilidade específica, promovendo:

* Separação de responsabilidades
* Escalabilidade
* Organização do código
* Facilidade de manutenção

O **Gateway** atua como ponto de entrada único, direcionando as requisições para os serviços correspondentes.
