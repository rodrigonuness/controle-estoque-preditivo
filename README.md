# Sistema de Controle de Estoque Preditivo

## 📦 Sobre o Projeto
Este sistema foi desenvolvido como parte de um projeto acadêmico na **CESAR School**, com o objetivo de criar uma solução completa para **controle de estoque** com **previsão de demanda**, utilizando conceitos de **DDD (Domain-Driven Design)**, **arquitetura limpa** e **padrões de projeto**.

O sistema permite gerenciar entradas e saídas de produtos, calcular **pontos de ressuprimento** (*reorder point*), prever demandas futuras com base no histórico de vendas e gerar pedidos automáticos para fornecedores.

---

## 🚀 Funcionalidades Principais
- **Movimentação de estoque** (entrada, saída e ajuste)
- **Previsão de demanda** com múltiplas estratégias (média móvel, suavização exponencial, etc.)
- **Cálculo de reorder point e lead time**
- **Geração automática de pedidos** com cotação a múltiplos fornecedores
- **Alertas de estoque baixo** (Observer Pattern)
- **Gestão de fornecedores e prazos**
- **Relatórios de ruptura e análise ABC**

---

## 🛠 Tecnologias Utilizadas
- **Backend:** Java, Spring Boot, Spring Data JPA
- **Frontend:** Angular
- **Banco de Dados:** MySQL
- **Testes:** JUnit 5, Cucumber (BDD)
- **Outros:** Docker Compose, Context Mapper, Flyway

---

## 🧩 Arquitetura
O sistema segue **Arquitetura Limpa**, separando regras de negócio da infraestrutura e utilizando **DDD** com múltiplos *bounded contexts*:
- **Estoque**
- **Previsão**
- **Compras**
- **Fornecedores**
- **Notificações**

Padrões de projeto aplicados:
- **Strategy** – escolha do método de previsão de demanda
- **Observer** – alertas de estoque
- **Template Method** – fluxo de pedidos automáticos

---

## 📌 Como Executar
### Pré-requisitos
- [Java 17+](https://adoptium.net/)
- [Node.js 18+](https://nodejs.org/)
- [Docker](https://www.docker.com/)

### Passos
1. Clone o repositório:
```bash
git clone https://github.com/rodrigonuness/controle-estoque-inteligente.git
