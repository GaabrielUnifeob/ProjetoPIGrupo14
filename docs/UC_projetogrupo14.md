# Documentação de Casos de Uso – Sabor do Campo

---

## 1. Introdução

Este documento descreve os casos de uso do aplicativo mobile desenvolvido para a empresa **Sabor do Campo**, com foco no controle de estoque de produtos hortifrúti, como couve e milho.

O objetivo é detalhar as interações entre os usuários e o sistema, garantindo clareza no funcionamento da aplicação.

---

## 2. Atores do Sistema

| Ator | Descrição |
|------|----------|
| Usuário | Funcionário ou gestor responsável pelo controle de estoque, pedidos e operações |

---

## 3. Lista de Casos de Uso

- Realizar Login  
- Cadastrar Produto  
- Registrar Entrada de Estoque  
- Registrar Saída (Venda)  
- Consultar Estoque  
- Cadastrar Pedido  
- Gerenciar Entregas  
- Registrar Pagamento  
- Visualizar Dashboard  

---

## 4. Descrição dos Casos de Uso

---

### 4.1 Realizar Login

**Ator:** Usuário  
**Descrição:** Permite acesso ao sistema de forma segura  
**Pré-condições:** Usuário cadastrado  
**Pós-condições:** Usuário autenticado  

**Fluxo Principal:**
1. Usuário abre o aplicativo  
2. Informa login e senha  
3. Sistema valida credenciais  
4. Acesso liberado  

**Fluxos Alternativos:**
- Senha incorreta → exibir erro  
- Usuário não encontrado → acesso negado  
- Falha de conexão → informar usuário  

---

### 4.2 Cadastrar Produto

**Ator:** Usuário  
**Descrição:** Permite cadastrar produtos (couve/milho)  
**Pré-condições:** Usuário autenticado  
**Pós-condições:** Produto registrado  

**Fluxo Principal:**
1. Acessa tela de cadastro  
2. Informa nome, tipo e quantidade  
3. Confirma cadastro  
4. Sistema salva produto  

**Fluxos Alternativos:**
- Campos vazios → solicitar preenchimento  
- Produto duplicado → exibir alerta  

---

### 4.3 Registrar Entrada de Estoque

**Ator:** Usuário  
**Descrição:** Adiciona produtos ao estoque  
**Pré-condições:** Produto cadastrado  
**Pós-condições:** Estoque atualizado  

**Fluxo Principal:**
1. Seleciona produto  
2. Informa quantidade  
3. Confirma operação  
4. Sistema atualiza estoque  

**Fluxos Alternativos:**
- Quantidade inválida → bloquear operação  
- Produto inexistente → erro  

---

### 4.4 Registrar Saída (Venda)

**Ator:** Usuário  
**Descrição:** Registra venda de produtos  
**Pré-condições:** Produto disponível  
**Pós-condições:** Estoque reduzido  

**Fluxo Principal:**
1. Seleciona produto  
2. Informa quantidade  
3. Confirma  
4. Sistema atualiza estoque  

**Fluxos Alternativos:**
- Estoque insuficiente → operação negada  
- Produto não encontrado → erro  

---

### 4.5 Consultar Estoque

**Ator:** Usuário  
**Descrição:** Exibe produtos e quantidades  
**Pré-condições:** Usuário autenticado  

**Fluxo Principal:**
1. Acessa tela de estoque  
2. Sistema exibe lista  

**Fluxos Alternativos:**
- Nenhum produto → exibir mensagem  

---

### 4.6 Cadastrar Pedido

**Ator:** Usuário  
**Descrição:** Registra pedidos  
**Pré-condições:** Produtos cadastrados  
**Pós-condições:** Pedido salvo  

**Fluxo Principal:**
1. Inicia pedido  
2. Seleciona produtos  
3. Confirma  
4. Sistema registra  

**Fluxos Alternativos:**
- Produto sem estoque → aviso  
- Dados incompletos → bloquear  

---

### 4.7 Gerenciar Entregas

**Ator:** Usuário  
**Descrição:** Atualiza status de entrega  
**Pré-condições:** Pedido existente  

**Fluxo Principal:**
1. Seleciona pedido  
2. Atualiza status  
3. Sistema salva  

**Fluxos Alternativos:**
- Pedido não encontrado → erro  

---

### 4.8 Registrar Pagamento

**Ator:** Usuário  
**Descrição:** Registra pagamento  
**Pré-condições:** Pedido existente  

**Fluxo Principal:**
1. Seleciona pedido  
2. Informa pagamento  
3. Confirma  
4. Sistema salva  

**Fluxos Alternativos:**
- Pedido inexistente → erro  

---

### 4.9 Visualizar Dashboard

**Ator:** Usuário  
**Descrição:** Exibe indicadores  

**Fluxo Principal:**
1. Acessa dashboard  
2. Sistema mostra dados  

**Fluxos Alternativos:**
- Sem dados → exibir mensagem  

---

## 5. Relação entre Casos de Uso e MVP

### Funcionalidades do MVP

| Funcionalidade | Caso de Uso | Descrição |
|---------------|------------|----------|
| Login | Realizar Login | Acesso ao sistema |
| Cadastro de produtos | Cadastrar Produto | Registro de produtos |
| Entrada de estoque | Registrar Entrada de Estoque | Adição de produtos |
| Saída de estoque | Registrar Saída (Venda) | Baixa no estoque |
| Consulta de estoque | Consultar Estoque | Visualização do estoque |

---

### Funcionalidades Futuras

| Funcionalidade | Caso de Uso | Justificativa |
|---------------|------------|--------------|
| Pedidos | Cadastrar Pedido | Evolução do sistema |
| Entregas | Gerenciar Entregas | Depende de pedidos |
| Pagamentos | Registrar Pagamento | Complemento |
| Dashboard | Visualizar Dashboard | Análise gerencial |

---

## 6. Conclusão

Os casos de uso apresentados representam as principais funcionalidades do sistema Sabor do Campo.

O MVP foi definido com foco no controle de estoque, garantindo uma entrega inicial eficiente. As demais funcionalidades serão implementadas em fases futuras, permitindo evolução contínua do sistema.

---
