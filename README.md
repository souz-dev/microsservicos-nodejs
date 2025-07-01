# 🧩 Microsserviços com Node.js, Docker, RabbitMQ e Kong — Projeto de Estudos

Este repositório contém um projeto de estudos que simula uma arquitetura baseada em **microsserviços**, utilizando tecnologias como **Node.js**, **Docker**, **RabbitMQ** e **Kong**. O objetivo é experimentar conceitos como separação de domínios, mensageria assíncrona e infraestrutura desacoplada.

---

## 📁 Estrutura do Projeto

```bash
├── app-invoices/ # Microsserviço responsável por faturas
├── app-orders/ # Microsserviço responsável por pedidos
├── contracts/ # Contratos e tipos compartilhados entre serviços
├── docker/ # Configurações auxiliares de Docker e Kong
├── infra/ # Infraestrutura e provisionamento (ex: scripts, volumes)
├── docker-compose.yml # Orquestração dos serviços
└── exemplo-com-dominio-e-secret-manager.ts # Exemplo extra de domínio e secrets

```


---

## 🚀 Tecnologias Utilizadas

- **Node.js** – execução dos microsserviços
- **Docker / Docker Compose** – orquestração dos containers
- **RabbitMQ** – comunicação assíncrona entre serviços
- **Kong** – API Gateway para gerenciamento centralizado
- **TypeScript** – tipagem estática no código (presente em alguns serviços)
- **MongoDB / PostgreSQL** *(caso esteja em uso nos serviços)*

---

## 🧪 Funcionalidades Demonstradas

- Separação de responsabilidades por serviço (`orders` e `invoices`)
- Comunicação via **mensageria assíncrona com RabbitMQ**
- Compartilhamento de contratos e tipos via pasta `contracts`
- Gateway de entrada com **Kong**
- Gerenciamento de secrets e domínios (arquivo de exemplo incluído)

---

## 🧰 Como Executar

1. **Clone o repositório**

```bash
git clone https://github.com/seu-usuario/microservice-aula.git
cd microservice-aula
