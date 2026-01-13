# REST Spring Application Lab

Este repositório é um laboratório prático projetado para explorar, testar e implementar conceitos avançados do ecossistema **Spring Boot 3**. O foco principal é a integração de dependências essenciais para o desenvolvimento de APIs corporativas robustas, escaláveis e seguras.

---

## 🛠️ Tecnologias e Stack Técnica

O projeto utiliza **Java 21** e está estruturado com as seguintes tecnologias:

### 🚀 Core & API Design
* **Spring Boot 3.5.x**: Base da aplicação.
* **SpringDoc OpenAPI (Swagger)**: Documentação interativa e testes de endpoints via interface web.
* **HATEOAS**: Implementação de links hipermídia para navegabilidade da API.
* **Content Negotiation**: Suporte a múltiplos formatos de dados (**JSON, XML e YAML**).

### 🔐 Segurança
* **Spring Security**: Estrutura de segurança e controle de acesso.
* **Java JWT (Auth0)**: Implementação de autenticação stateless via tokens JWT.

### 🗄️ Persistência e Migrações
* **Spring Data JPA**: Abstração da camada de dados e persistência.
* **MySQL**: Banco de dados relacional.
* **Flyway Migration**: Controle de versionamento do esquema do banco de dados.
* **Dozer Mapper**: Mapeamento inteligente entre Entidades e DTOs.

### 📊 Relatórios e Documentos
* **JasperReports**: Motor para geração de relatórios complexos e exportação em PDF.
* **Apache POI & Commons CSV**: Manipulação de planilhas Excel (OOXML) e arquivos CSV.
* **ZXing (Zebra Crossing)**: Geração e leitura de QR Codes e códigos de barras.

### 🧪 Testes e Qualidade
* **Testcontainers (MySQL)**: Levantamento de instâncias reais de banco de dados em containers Docker para testes de integração.
* **REST Assured**: Validação fluente de endpoints e respostas HTTP.
* **Spring Boot Starter Test**: Testes unitários e de integração com JUnit 5.

---

## ⚙️ Configuração e Execução

### Pré-requisitos
* **Java 21** instalado.
* **Maven 3.9+** para gerenciamento de dependências.
* **Docker** (necessário para rodar os Testcontainers).

### Variáveis de Ambiente
O plugin do Flyway está configurado para ler as credenciais do banco de dados do seu sistema. Defina as seguintes variáveis:
* `usernameDB`: Seu usuário do banco.
* `passwordDB`: Sua senha do banco.

### Comandos Úteis
1.  **Compilar o projeto:**
    ```bash
    mvn clean install
    ```
2.  **Executar Migrations do Flyway:**
    ```bash
    mvn flyway:migrate
    ```
3.  **Rodar a aplicação:**
    ```bash
    mvn spring-boot:run
    ```
4.  **Executar Testes:**
    ```bash
    mvn test
    ```

---

## 📧 Outros Recursos Integrados
* **Spring Mail**: Suporte para envio de notificações por e-mail.
* **Spring DevTools**: Facilita o desenvolvimento com LiveReload e Restart automático.

---
> **Nota:** Este é um projeto de estudo pessoal. Sinta-se à vontade para explorar os pacotes e as implementações.
