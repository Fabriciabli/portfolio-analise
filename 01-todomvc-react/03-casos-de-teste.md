<h1 align="center">Casos de Teste – TodoMVC</h1>

## 🧪 Suíte 1 – Tela Inicial

**Tipo de Teste:** Funcional  
**Subtipo de Teste:** Caso de teste  
**Objetivo do Teste:** Validar a tela inicial  
**Protótipo:** [TODOMVC](https://todomvc.com/examples/react/dist/)  
**Pré-condição:** Nenhuma 
**Dados Necessários:**  Nenhum 
**Requisitos:** Tela inicial


| ID  | Critério de Aceite | Prioridade | Severidade | Resultado Esperado | Resultado Obtido | Defeitos | Status |
|-----|---------------------|------------|------------|--------------------|------------------|----------|--------|
| 9   | DADO que estou na tela inicial | Alta | Médio | ENTÃO o campo de input está disponível na tela e deve conter a mensagem "What needs to be done?" | OK | – | 😀 |

---

## 🧪 Suíte 2 – Adicionar itens

**Objetivo do Teste:** Validar a inclusão de itens da lista
**Requisitos:** Adicionar itens

| ID | Critério de Aceite | Prioridade | Severidade | Resultado Esperado | Resultado Obtido | Defeitos | Status |
|----|---------------------|------------|------------|--------------------|------------------|----------|--------|
| 10 | DADO que insiro o item e clico em enter | Alta | Alta | O item deve ser exibido na lista | OK | – | 😀 |
| 11 | DADO que possuo ao menos um item | Baixa | Baixo | Ícone de seleção deve aparecer à esquerda | OK | – | 😀 |
| 12 | DADO que passo o mouse sobre o item | Baixa | Baixo | Deve aparecer um "X" vermelho para excluir | OK | – | 😀 |
| 13 | DADO que a lista foi criada | Alta | Alta | Um rodapé deve ser exibido | OK | – | 😀 |
| 14 | DADO que o rodapé é exibido | Alta | Alta | Deve conter contador e filtros | OK | – | 😀 |

---

## 🧪 Suíte 3 – Filtrar itens todos
  
**Objetivo do Teste:** Validar a funcionalidade filtrar todos
**Requisitos:** Validar filtro - todos

| ID | Critério de Aceite | Prioridade | Severidade | Resultado Esperado | Resultado Obtido | Defeitos | Status |
|----|---------------------|------------|------------|--------------------|------------------|----------|--------|
| 15 | DADO que possuo itens concluídos e a fazer | Média | Médio | Os ativos sem marcação e os concluídos riscados e em cinza | OK | – | 😀 |
| 16 | DADO que clico em "All" com itens não concluídos | Baixa | Baixo | Itens não concluídos estão visíveis e sem marcação | OK | – | 😀 |

---

## 🧪 Suíte 4 – Filtro ativo

**Objetivo do Teste:** Validar a funcionalidade de itens ativos
**Requisitos:** Validar filtro - ativos

| ID | Critério de Aceite | Prioridade | Severidade | Resultado Esperado | Resultado Obtido | Defeitos | Status |
|----|---------------------|------------|------------|--------------------|------------------|----------|--------|
| 17 | DADO que clico em "Active" | Média | Médio | Itens a fazer são exibidos e contador mostra ativos | OK | – | 😀 |
| 18 | DADO que clico em um item ativo | Baixa | Baixo | Item desaparece da tela "Active", contador ajustado | OK | – | 😀 |
| 19 | DADO que concluo ou excluo todos itens | Baixa | Baixo | Tela "Active" fica em branco e contador zera | OK | – | 😀 |

---

## 🧪 Suíte 5 – Filtro concluído
 
**Objetivo do Teste:** Validar a funcionalidade de itens concluídos
**Requisitos:** Validar filtro - concluído

| ID | Critério de Aceite | Prioridade | Severidade | Resultado Esperado | Resultado Obtido | Defeitos | Status |
|----|---------------------|------------|------------|--------------------|------------------|----------|--------|
| 20 | DADO que clico em "Completed" | Média | Médio | Itens concluídos são exibidos e contador mostra ativos | OK | – | 😀 |
| 21 | DADO que desmarco um item | Baixa | Baixo | Item volta para ativo, desaparece da tela | OK | – | 😀 |
| 22 | DADO que clico em excluir | Baixa | Baixo | Itens somem, tela limpa, contador atualizado | OK | – | 😀 |

---

## 🧪 Suíte 6 – Itens unitário

**Objetivo do Teste:** Validar a Conclusão de itens unitário
**Requisitos:** Conclusão de itens - unitária

| ID | Critério de Aceite | Prioridade | Severidade | Resultado Esperado | Resultado Obtido | Defeitos | Status |
|----|---------------------|------------|------------|--------------------|------------------|----------|--------|
| 23 | DADO que marco um item | Alta | Alta | Item aparece em "Completed", contador atualiza | OK | – | 😀 |
| 24 | DADO que desmarco o item | Baixa | Baixo | Item volta como ativo, desaparece da lista concluída | OK | – | 😀 |
| 25 | DADO que excluo um item concluído | Baixa | Baixo | Item desaparece, contador permanece com ativos | OK | – | 😀 |

---

## 🧪 Suíte 7 – Itens lotes

**Objetivo do Teste:** Validar a Conclusão de itens em lotes
**Requisitos:** Conclusão de itens - em lotes

| ID | Critério de Aceite | Prioridade | Severidade | Resultado Esperado | Resultado Obtido | Defeitos | Status |
|----|---------------------|------------|------------|--------------------|------------------|----------|--------|
| 26 | DADO que marco todos os itens | Alta | Alta | Lista concluída exibida e contador zerado | OK | – | 😀 |
| 27 | DADO que clico no check geral | Média | Médio | Todos os itens são reativados, contador mostra ativos | OK | – | 😀 |

---

## 🧪 Suíte 8 – Itens finalizados
 
**Objetivo do Teste:** Validar a Conclusão de itens finalizados
**Requisitos:** Limpar itens finalizados

| ID | Critério de Aceite | Prioridade | Severidade | Resultado Esperado | Resultado Obtido | Defeitos | Status |
|----|---------------------|------------|------------|--------------------|------------------|----------|--------|
| 28 | DADO que clico em "Clear completed" | Baixíssima | Baixo | Itens concluídos desaparecem, input limpo | OK | – | 😀 |