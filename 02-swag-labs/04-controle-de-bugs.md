# 🐞 Controle de Defeitos – Swag Labs


## 📋 Informações do Projeto

- **Cliente:** Swag Labs – [https://www.saucedemo.com/](https://www.saucedemo.com/v1/index.html)
- **Ponto Focal:** Fabrícia Fernnades, @fabricia.fernandes  
- **E-mail:** fabriciaqa@gmail.com  
- **Objetivo do Projeto:** Validar o plano de Teste v2.0
- **Público Alvo:** Usuários do site Saucedemo  
- **Analista de Teste Responsável:** Fabrícia Fernandes, @fabricia.fernandes 
- **E-mail do Analista:** fabriciaqa@gmail.com 
- **Project Manager:** —  
- **Data de Início:** 03/06/2025  
- **Data de Término:** 03/06/2025

---

## 🎯 Propósito

Validar a não ocorrência de defeitos e a conformidade das funcionalidades previstas no Plano de Teste.

**Escopo:** Todas as funcionalidades listadas no respectivo plano.  
**Referências:** Plano de Teste v2.0

---

## 🐞 Controle de Defeitos

| ID    | Defeito | Descrição | Story / ID | Versão | Prioridade | Severidade | Time | Status |
|-------|---------|-----------|------------|--------|------------|------------|------|--------|
| D009  | Menu possui itens não esperados | DADO que estou logado QUANDO clico no menu ENTÃO deve ser exibido as três opções - All Items - About - Logout MAS a opção Reset App State está sendo exibida | REQ 2 – Validar o Menu do site / ID09 | 002 | Médio | Médio | FrontEnd | 😟 |
| D016  | Produto não é adicionado ao carrinho | DADO que estou na aplicação E visualizo o item desejado QUANDO clico em "add cart" ENTÃO o item deveria ser adicionado MAS ao clicar, nada acontece | REQ 3 – Adicionar itens ao carrinho / ID16 | 001 | Alto | Crítico | BackEnd | 😟 |
| D017  | Redirecionamento incorreto ao clicar no item | DADO que estou na aplicação E visualizo o item desejado QUANDO clico no item ENTÃO a tela correta deveria ser exibida MAS redireciona para outro produto não relacionado | REQ 3 – Adicionar itens ao carrinho / ID17 | 001 | Alto | Alta | FrontEnd | 😐 |
| D019  | Descrição de produto com chamada de função | DADO que itens foram adicionados QUANDO clico no carrinho ENTÃO os itens e contador devem ser exibidos corretamente MAS a descrição do item 01 mostra uma função ao invés do texto | REQ 3 – Adicionar itens ao carrinho / ID19 | 001 | Alto | Crítico | BackEnd | 😟 |
| D024  | Erro ao aplicar filtro | DADO que estou em filtro QUANDO seleciono uma opção ENTÃO os itens deveriam ser ordenados MAS um pop-up de erro aparece: "Sorting is broken! This error has been reported to Backtrace." | REQ 5 – Filtros / ID24 | 001 | Médio | Baixo | BackEnd | 😐 |

---