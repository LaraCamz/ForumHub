# 🚀 ForumHub

**Uma plataforma de fórum REST API desenvolvida como challenge da Alura**

ForumHub é um sistema de gerenciamento de fórum construído com **Spring Boot** e **Java 21**, oferecendo funcionalidades completas de criação, leitura e gerenciamento de tópicos e respostas em um ambiente controlado e seguro.

---

## 📌 Funcionalidades

- ✅ **Autenticação e Autorização**: Sistema seguro com tokens JWT
- ✅ **Gerenciamento de Tópicos**: Criar, listar, atualizar e deletar tópicos
- ✅ **Sistema de Respostas**: Responder a tópicos com rastreamento de autoria
- ✅ **Controle de Usuários**: Gerenciamento de perfis e permissões
- ✅ **API RESTful**: Endpoints padronizados e documentados
- ✅ **Persistência de Dados**: Banco de dados relacional com JPA/Hibernate

---

## 🛠️ Tecnologias Utilizadas

| Tecnologia | Versão | Descrição |
|-----------|--------|-----------|
| **Java** | 21 | Linguagem de programação |
| **Spring Boot** | 3.x | Framework web |
| **Spring Security** | - | Autenticação e autorização |
| **Spring Data JPA** | - | ORM e acesso a dados |
| **Maven** | - | Gerenciador de dependências |
| **MySQL/PostgreSQL** | - | Banco de dados relacional |
| **JWT** | - | Tokens de autenticação |

---

## 🚀 Como Executar

### Pré-requisitos

- Java 21 ou superior instalado
- Maven 3.8+
- Banco de dados MySQL (ou PostgreSQL)
- IDE recomendada: IntelliJ IDEA ou VS Code

### Instalação

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/LaraCamz/ForumHub.git
   cd ForumHub

   Configure o banco de dados:

2. Crie um banco de dados chamado forumhub_db
3. Atualize as credenciais em src/main/resources/application.properties:
properties:

spring.datasource.url=jdbc:mysql://localhost:3306/forumhub_db
spring.datasource.username=seu_usuario
spring.datasource.password=sua_senha
Instale as dependências:

bash
mvn clean install
Execute a aplicação:

bash
mvn spring-boot:run
A aplicação estará disponível em http://localhost:8080

📡 API REST - Exemplos de Requisições
Autenticação
POST /auth/login

JSON
{
  "email": "usuario@example.com",
  "senha": "senha123"
}
Tópicos
GET /topicos - Listar todos os tópicos

POST /topicos - Criar novo tópico

JSON
{
  "titulo": "Como usar Spring Boot?",
  "mensagem": "Estou iniciando com Spring Boot...",
  "nomeCurso": "Java Backend"
}
GET /topicos/{id} - Obter tópico específico

PUT /topicos/{id} - Atualizar tópico

DELETE /topicos/{id} - Deletar tópico

Respostas
GET /topicos/{id}/respostas - Listar respostas de um tópico

POST /topicos/{id}/respostas - Adicionar resposta

JSON
{
  "mensagem": "Excelente pergunta! Aqui está a resposta..."
}
🔐 Autenticação
O ForumHub utiliza JWT (JSON Web Tokens) para autenticação:

Faça login com suas credenciais
Receba um token JWT
Inclua o token no header de autorização:
Code
Authorization: Bearer seu_token_jwt_aqui
🧪 Testes
Execute os testes automatizados com:

bash
mvn test
📚 Documentação API
A documentação interativa da API está disponível em:

Swagger UI: http://localhost:8080/swagger-ui.html
OpenAPI: http://localhost:8080/v3/api-docs
🔄 Fluxo de Desenvolvimento
Este projeto segue a metodologia de commits semânticos:

feat: - Novas funcionalidades
fix: - Correção de bugs
docs: - Mudanças na documentação
style: - Formatação de código
refactor: - Refatoração de código
🎯 Próximos Passos / Melhorias Futuras
 Implementar sistema de notificações por email
 Adicionar busca avançada com Elasticsearch
 Criar interface web com React/Vue
 Implementar sistema de rating/reputação
 Adicionar suporte a múltiplos idiomas
 Implementar cache com Redis
 Adicionar integração com OAuth2
🤝 Contribuições
Contribuições são bem-vindas! Para contribuir:

Faça um fork do projeto
Crie uma branch para sua feature (git checkout -b feature/AmazingFeature)
Commit suas mudanças (git commit -m 'Add some AmazingFeature')
Push para a branch (git push origin feature/AmazingFeature)
Abra um Pull Request
📄 Licença
Este projeto está disponível sob licença MIT.

👩‍💻 Autor
Lara Camile Ferreira Lima

GitHub: @LaraCamz
Email: seu-email@example.com
📞 Suporte
Tem dúvidas ou encontrou um bug? Abra uma issue no repositório!
