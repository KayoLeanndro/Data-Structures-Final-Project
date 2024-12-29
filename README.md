# Gerenciador de Tarefas

## Descrição
Este projeto implementa um gerenciador de tarefas simples, porém poderoso, utilizando diversas estruturas de dados para organizar e manipular as tarefas. O sistema permite aos usuários adicionar, visualizar, buscar, remover e marcar tarefas como concluídas.

---

## Funcionalidades Principais

### Adição de Tarefas
- Cada tarefa possui:
  - **Título**
  - **Descrição**
  - **Prioridade**: alta, média ou baixa.
- As tarefas são armazenadas em uma **lista encadeada** para flexibilidade.

### Visualização de Tarefas
- As tarefas são exibidas de forma organizada por prioridade, utilizando uma **fila de prioridade**.

### Remoção de Tarefas
- Possibilidades:
  - Remover uma tarefa pelo título.
  - Remover a tarefa mais urgente.

### Busca de Tarefas
- Busca eficiente por título utilizando uma **tabela hash**.

### Histórico de Tarefas Concluídas
- As tarefas concluídas são armazenadas em uma **pilha**, permitindo desfazer a última tarefa marcada como concluída.

---

## Estruturas de Dados Utilizadas

- **Lista Encadeada**: Armazena todas as tarefas.
- **Fila de Prioridade**: Organiza as tarefas por prioridade.
- **Pilha**: Armazena o histórico de tarefas concluídas.
- **Tabela Hash**: Permite busca rápida por título.

---

## Exemplo de Interação

### Adicionar Tarefas
- Tarefa 1: **"Estudar para a prova de algoritmos"** - Prioridade **Alta**  
- Tarefa 2: **"Comprar pão e leite"** - Prioridade **Baixa**  
- Tarefa 3: **"Responder e-mails do trabalho"** - Prioridade **Média**

### Exibir Tarefas
```plaintext
[Alta] Estudar para a prova de algoritmos  
[Média] Responder e-mails do trabalho  
[Baixa] Comprar pão e leite
```

### Buscar Tarefa
```plaintext
Buscar: "Responder e-mails"
Resultado: [Média] Responder e-mails do trabalho - "Responder aos e-mails pendentes do cliente X."
```

### Estrutura do Código
```plaintext
#### Classes e Métodos
- Tarefa: Representa uma tarefa individual.
- ListaEncadeada: Gerencia a lista de todas as tarefas.
- FilaDePrioridade: Organiza as tarefas por prioridade.
- PilhaDeHistorico: Armazena o histórico de tarefas concluídas.
- TabelaHashDeTarefas: Permite busca eficiente por título.
```
```plaintext
Fluxo Principal
Menu interativo para o usuário com as seguintes opções:
Adicionar tarefa.
Visualizar tarefas.
Buscar tarefa.
Remover tarefa.
Marcar tarefa como concluída.
Desfazer conclusão de tarefa.
```

### Desafios Extras
```plaintext
Persistência de Dados em Java:

Utilize bibliotecas como JDBC ou Hibernate para salvar e carregar tarefas de um banco de dados (e.g., SQLite, PostgreSQL).
Alternativamente, salve as tarefas em arquivos (e.g., JSON ou XML) para persistência local.
Interface Gráfica ou Web com Java:

Crie uma interface visual mais intuitiva utilizando JavaFX ou Swing.
Para uma solução web, utilize frameworks como Spring Boot ou Vaadin.
Ordenação de Prioridade:

Explore outras estruturas de dados, como árvores binárias de busca ou heaps, para otimizar a ordenação por prioridade.
```
