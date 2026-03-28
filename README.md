# Calendário Operacional RH

Aplicação web para gestão de rotinas operacionais de Recursos Humanos e Departamento Pessoal em formato de calendário mensal, com foco em simplicidade, visualização clara e controle prático do dia a dia.

---

## 1. Objetivo do projeto

O Calendário Operacional RH foi criado para resolver um problema comum em RH/DP:

> "As atividades existem, mas não estão organizadas visualmente por data, prioridade e responsável."

O sistema transforma sua operação em uma visão simples:
- o mês inteiro visível
- atividades dentro de cada dia
- status claro
- possibilidade de ajuste rápido

Ele funciona como um **painel operacional vivo**.

---

## 2. Conceito do produto

O sistema segue 3 pilares:

### 2.1 Visualização
Tudo está no calendário:
- você vê o mês inteiro
- entende carga de trabalho por dia
- identifica gargalos rapidamente

### 2.2 Manipulação rápida
Sem burocracia:
- clicar → editar
- botão → mover tudo
- checkbox → marcar pagamento

### 2.3 Persistência simples
Sem banco de dados:
- tudo salvo no navegador (`localStorage`)
- exportação e importação via JSON

---

## 3. Funcionalidades principais

### 3.1 Cadastro de atividades
Cada atividade contém:
- data
- título
- responsável
- categoria
- observações
- status
- flag de pagamento

---

### 3.2 Status operacional

| Código | Nome         | Uso prático                         |
|--------|-------------|------------------------------------|
| todo   | A Fazer     | ainda não iniciado                 |
| doing  | Em andamento| execução em curso                  |
| done   | Concluído   | finalizado                         |
| late   | Atrasado    | passou do prazo                    |

---

### 3.3 Marcação de pagamento

Uma atividade pode ter:

```json
"pagamento": true
