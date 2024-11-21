# Desafio Técnico de Backend (PHP - Laravel)

## Objetivo Geral

Desenvolver uma API REST simples e funcional utilizando PHP (com o framework Laravel) para gerenciar uma lista de tarefas. Este desafio foi projetado para avaliar habilidades em backend, incluindo estruturação de código, boas práticas de programação, segurança, e a implementação de testes automatizados.

## Descrição do Projeto

A aplicação deve implementar um sistema de gerenciamento de tarefas, com as seguintes funcionalidades:

- CRUD de Tarefas:
  -	Criar uma nova tarefa.
  -	Listar todas as tarefas.
  -	Visualizar os detalhes de uma tarefa específica.
  -	Atualizar uma tarefa existente.
  -	Excluir uma tarefa.
- Detalhes da Tarefa:
  -	Uma tarefa deve conter:
  -	id (gerado automaticamente, UUID preferido).
  -	title (obrigatório, texto).
  -	description (opcional, texto longo).
  -	status (enum: pending, in_progress, completed).
  -	created_at e updated_at.
- Filtros na Listagem:
  -	Permitir filtrar as tarefas pelo status.
- Validação de Dados:
  -	Valide os dados de entrada para garantir a consistência e segurança.
- Tratamento de Erros:
  -	Responda com mensagens claras e códigos HTTP apropriados.

## Expectativas Técnicas

### Estrutura do Código

-	Utilize boas práticas de design, preferencialmente DDD (Domain-Driven Design).
-	Separe camadas como Controllers, Services, Repositories, e Models.

### Segurança

-	Implemente as práticas básicas de segurança:
-	Validação e sanitização de entradas.
-	Utilize UUIDs para evitar previsibilidade de IDs.

### Testes Automatizados

-	Crie testes automatizados para as funcionalidades principais:
-	Testes de unidade para métodos isolados.
-	Testes de integração para endpoints.

### Critérios de Avaliação

-	Funcionalidade:
  -	O sistema atende aos requisitos funcionais?
-	Organização e Estrutura do Código:
  -	Código limpo, legível e bem organizado.
-	Aderência a Boas Práticas:
  -	Padrões de projeto, SOLID, e uso adequado do framework.
-	Segurança:
  -	Cuidados com a validação de dados e outras práticas básicas.
-	Testes Automatizados:
  -	Qualidade e abrangência dos testes.
-	Documentação:
  -	Breve descrição no README sobre as decisões de design, como rodar o projeto e executar os testes.

### Guia de Implementação

- Setup
  -	Configure um projeto Laravel.
  -	Utilize o comando artisan para gerar os recursos necessários.

- Funcionalidades
  -	Rotas:
    -	/api/tasks (GET) - Listar todas as tarefas.
    -	/api/tasks?status={status} (GET) - Filtrar tarefas por status.
    -	/api/tasks/{id} (GET) - Obter detalhes de uma tarefa.
    -	/api/tasks (POST) - Criar uma nova tarefa.
    -	/api/tasks/{id} (PUT) - Atualizar uma tarefa.
    -	/api/tasks/{id} (DELETE) - Excluir uma tarefa.
  -	Validação:
    -	Use FormRequest ou validações no controlador para garantir a consistência.
  -	Respostas:
    -	Padronize as respostas d
