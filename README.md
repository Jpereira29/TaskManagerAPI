# TaskManager API - EP2

Este projeto consiste em uma API RESTful desenvolvida em .NET. A API **TaskManager** permite gerenciar uma lista de tarefas, suportando operações de criação, leitura, atualização e exclusão (CRUD).

## Time

-  Cícero Jeferson Santos de Araújo 2023011591
-  Francisco Airton Araújo Júnior 2023010960
-  Jorge Pereira de Oliveira 2023011027

## Tecnologias Utilizadas

-   **.NET 9**
-   **ASP.NET Core Web API**
-   **Swagger (OpenAPI)** para documentação e testes.

## Como Executar e Testar Localmente

Siga as instruções abaixo para executar a API em sua máquina local.

### Pré-requisitos

-   [.NET SDK 9.0](https://dotnet.microsoft.com/download) instalado.

### Passos para Execução

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/Jpereira29/TaskManagerAPI
    cd TaskManager
    ```

2.  **Execute a aplicação:**
    Abra um terminal na raiz do projeto (`TaskManager`) e execute o seguinte comando:
    ```bash
    dotnet run
    ```

3.  **Acesse a API:**
    A aplicação estará rodando localmente. O terminal indicará a URL - `https://localhost:7015`.

## Documentação da API

A documentação completa e interativa da API foi gerada utilizando Swagger/OpenAPI e está disponível enquanto a aplicação está em execução.

-   **URL da Documentação:** [https://localhost:7015/swagger](https://localhost:7015/swagger)

Nesta página, você pode visualizar todas as rotas disponíveis, seus parâmetros, e testar cada uma delas diretamente do navegador.

## Exemplos de Requisição e Resposta

Aqui estão alguns exemplos de como interagir com a API.

### 1. Criar uma nova tarefa (POST)

**Requisição:**
-   Método: `POST`
-   URL: `https://localhost:7015/api/taskitem`
-   Corpo (Body) em JSON:
    ```json
    {
      "title": "Teste",
      "description": "Teste",
      "isCompleted": false
    }
    ```
---

## **[Componente Extensionista] Possíveis usos da nossa API**

O objetivo deste componente é conectar nosso projeto acadêmico a problemas do mundo real. Nossa API **TaskManager**, embora simples, serve para diversas aplicações práticas que podem ajudar tanto pessoas quanto negócios.

### **Para um Indivíduo (Estudante ou Profissional):**

Uma pessoa poderia usar essa API como o backend de um aplicativo de "To-Do List" pessoal. 
Imagine um aplicativo para celular ou desktop onde o usuário pode cadastrar suas tarefas diárias, marcar como concluídas e organizar suas atividades. 
A API seria responsável por armazenar e gerenciar esses dados de forma segura e eficiente. Isso ajudaria o usuário a aumentar sua produtividade e a não se esquecer de compromissos importantes.

### **Para um Negócio (Pequena Agência ou Startup):**

Uma pequena equipe de desenvolvimento ou uma agência de marketing poderia integrar nossa API a uma ferramenta de gerenciamento de projetos simples. 
Cada "tarefa" poderia representar uma demanda de um cliente ou uma etapa de um projeto interno. 
A API permitiria que diferentes sistemas consultassem e atualizassem o status das tarefas. 
Por exemplo, um gerente poderia criar uma nova tarefa pela interface web, e o desenvolvedor responsável receberia uma notificação automática via bot. 
Isso centraliza a comunicação, melhora a organização e ajuda a garantir que os prazos sejam cumpridos.
