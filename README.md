Este repositório apresenta um projeto desenvolvido para a criação de um Board de Tarefas utilizando Java e Spring Boot. O objetivo é fornecer uma aplicação simples e funcional para gerenciar tarefas, permitindo a criação, edição e remoção de tarefas de maneira eficiente.

## Tecnologias Utilizadas

- **Java 17**
- **Spring Boot 3**
- **Spring Web** (para exposição da API REST)
- **Spring Data JPA** (para interação com o banco de dados)
- **H2 Database** (banco de dados em memória para testes)
- **Lombok** (para redução de boilerplate no código)

## Funcionalidades

- Criar novas tarefas
- Listar todas as tarefas
- Atualizar tarefas existentes
- Excluir tarefas
- Buscar tarefas por ID

## Como Executar o Projeto

1. Clone este repositório:
   ```bash
   git clone https://github.com/Matheus-120/board-de-tarefas.git
   ```
2. Acesse a pasta do projeto:
   ```bash
   cd board-de-tarefas
   ```
3. Execute o projeto utilizando o Maven:
   ```bash
   mvn spring-boot:run
   ```
4. A API estará disponível em:
   ```
   http://localhost:8080
   ```

## Endpoints da API

### Criar uma nova tarefa
**POST** `/tarefas`
```json
{
  "titulo": "Estudar Java",
  "descricao": "Revisar conceitos de Spring Boot",
  "status": "PENDENTE"
}
```

### Listar todas as tarefas
**GET** `/tarefas`

### Buscar uma tarefa por ID
**GET** `/tarefas/{id}`

### Atualizar uma tarefa
**PUT** `/tarefas/{id}`
```json
{
  "titulo": "Estudar Java",
  "descricao": "Completar curso de Spring Boot",
  "status": "CONCLUIDO"
}
```

### Excluir uma tarefa
**DELETE** `/tarefas/{id}`

## Autor
Este projeto foi apresentado por **Matheus Ferreira**. Para mais informações, acesse o perfil no GitHub: [Matheus-120](https://github.com/Matheus-120).

