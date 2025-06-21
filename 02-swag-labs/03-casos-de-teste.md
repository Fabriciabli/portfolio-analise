<h1 align="center">Casos de Testes – Swag Labs</h1>


## 🧪 Suite 1 – Login

**Tipo de Teste:** Funcional  
**Subtipo:** Critério de Aceite  
**Objetivo:** Realizar login na aplicação  
**Pré-condição:**  
- Ter um usuário cadastrado  
- Ter uma senha cadastrada  

**Dados Necessários:**  
- Usuário com acesso: `standard_user`  
- Usuário bloqueado: `locked_out_user`  
- Senha: `secret_sauce`  

**Requisito:** REQ 1 - Funcionalidade login

| ID  | Critério de Aceite | Prioridade | Severidade | Resultado Esperado | Resultado Obtido | Defeitos | Status |
|-----|--------------------|------------|-------------|---------------------|-------------------|----------|--------|
| 6   | DADO que me encontro no navegador QUANDO acesso o site | Alto | Crítico | ENTÃO a tela de login deve ser exibida, com campos de usuário e senha, e botão de login | OK | — | 😀 |
| 7   | DADO que me encontro no site e adiciono standard_user e a senha secret_sauce QUANDO clico em logar | Médio | Médio | ENTÃO sou redirecionado para a Home da aplicação | OK | — | 😀 |
| 8   | DADO que me encontro no site e adiciono locked_out_user e a senha secret_sauce QUANDO clico em logar | Médio | Alta | ENTÃO não deve ser redirecionado à Home e deve exibir mensagem de usuário bloqueado | OK | — | 😀 |

---

## 🧪 Suite 2 – Validação do Menu

**Tipo de Teste:** Funcional  
**Subtipo:** Critério de Aceite  
**Objetivo:** Validar os itens do menu  
**Pré-condição:** Estar logado na aplicação  

**Dados Necessários:**  
- Usuário: `standard_user`  
- Senha: `secret_sauce`  

**Requisito:** REQ 2 - Validar o Menu do site

| ID  | Critério de Aceite | Prioridade | Severidade | Resultado Esperado | Resultado Obtido | Defeitos | Status |
|-----|--------------------|------------|-------------|---------------------|-------------------|----------|--------|
| 9   | DADO que estou logado QUANDO clico no menu | Médio | Médio | ENTÃO deve exibir: All Items, About, Logout | NOK | D009 | 😟 |
| 10  | DADO que estou logado e clico no menu QUANDO clico no "X" | Baixo | Baixo | ENTÃO o menu deve ser fechado | OK | — | 😀 |
| 11  | DADO que estou logado e clico no menu QUANDO clico fora do menu | Baixo | Baixo | ENTÃO o menu não deve ser fechado | OK | — | 😀 |
| 12  | DADO que estou fora da Home QUANDO clico em All Items | Baixo | Baixo | ENTÃO sou redirecionado para a Home | OK | — | 😀 |
| 13  | DADO que estou na aplicação QUANDO clico em Sobre | Baixo | Baixo | ENTÃO devo ser redirecionado para o site da empresa | OK | — | 😀 |
| 14  | DADO que estou na aplicação QUANDO clico em Logout | Médio | Médio | ENTÃO sou deslogado e redirecionado para login | OK | — | 😀 |

---

## 🧪 Suite 3 – Adicionar Itens ao Carrinho

**Tipo de Teste:** Funcional  
**Subtipo:** Critério de Aceite  
**Objetivo:** Adicionar itens ao carrinho  
**Pré-condição:**  
- Estar logado  
- Ter produtos disponíveis  

**Dados Necessários:**  
- Usuário: `problem_user`  
- Senha: `secret_sauce`  

**Requisito:** REQ 3 - Adicionar itens ao carrinho

| ID  | Critério de Aceite | Prioridade | Severidade | Resultado Esperado | Resultado Obtido | Defeitos | Status |
|-----|--------------------|------------|-------------|---------------------|-------------------|----------|--------|
| 15  | DADO que estou na home QUANDO clico em "add cart" | Alto | Crítico | ENTÃO o item é adicionado e contador incrementa +1 | OK | — | 😀 |
| 16  | DADO que vejo item desejado QUANDO clico em "add cart" | Alto | Crítico | ENTÃO item adicionado e contador +1 | NOK | D016 | 😟 |
| 17  | DADO que vejo item desejado QUANDO clico no item | Médio | Médio | ENTÃO exibe tela do item | NOK | D017 | 😐 |
| 18  | DADO que estou na tela do produto QUANDO clico em "add cart" | Médio | Médio | ENTÃO item adicionado, botão "remove" exibido | OK | — | 😀 |
| 19  | DADO que itens foram adicionados QUANDO clico no carrinho | Alto | Crítico | ENTÃO carrinho contém os itens e contador correto | NOK | D019 | 😐 |

---

## 🧪 Suite 4 – Remover Itens do Carrinho

**Tipo de Teste:** Funcional  
**Subtipo:** Critério de Aceite  
**Objetivo:** Remover itens do carrinho  
**Pré-condição:**  
- Estar logado  
- Ter itens adicionados  

**Dados Necessários:**  
- Usuário: `performance_glitch_user`  
- Senha: `secret_sauce`  

**Requisito:** REQ 4 - Remover itens do carrinho

| ID  | Critério de Aceite | Prioridade | Severidade | Resultado Esperado | Resultado Obtido | Defeitos | Status |
|-----|--------------------|------------|-------------|---------------------|-------------------|----------|--------|
| 20  | DADO que estou no carrinho e vejo itens QUANDO clico em "remove" | Alto | Crítico | ENTÃO item é removido e contador -1 | OK | — | 😀 |
| 21  | DADO que vejo item no carrinho QUANDO clico no item | Alto | Crítico | ENTÃO tela do item com botão "remove" é exibida | OK | — | 😀 |
| 22  | DADO que itens foram removidos QUANDO clico no carrinho | Alto | Crítico | ENTÃO carrinho atualizado sem os itens removidos | OK | — | 😀 |

---

## 🧪 Suite 5 – Filtro de Itens

**Tipo de Teste:** Funcional  
**Subtipo:** Critério de Aceite  
**Objetivo:** Filtrar itens  
**Pré-condição:**  
- Estar logado  
- Ter itens no sistema  

**Dados Necessários:**  
- Usuário: `error_user`  
- Senha: `secret_sauce`  

**Requisito:** REQ 5 - Filtrar itens no site

| ID  | Critério de Aceite | Prioridade | Severidade | Resultado Esperado | Resultado Obtido | Defeitos | Status |
|-----|--------------------|------------|-------------|---------------------|-------------------|----------|--------|
| 23  | DADO que estou na Home QUANDO clico no filtro | Baixo | Médio | ENTÃO opções de filtro são exibidas | OK | — | 😀 |
| 24  | DADO que estou no filtro QUANDO seleciono uma opção | Baixo | Médio | ENTÃO os itens são ordenados conforme o filtro | NOK | D024 | 😐 |
---
