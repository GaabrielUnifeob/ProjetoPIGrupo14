 DOCUMENTAÇÃO DE CASOS DE USO – Sabor do Campo
 
1. Caso de Uso: Realizar Login

Ator: Usuário (Funcionário/Gestor)
Descrição: Permite que o usuário acesse o sistema de forma segura.
Pré-condições: Usuário deve estar previamente cadastrado.
Pós-condições: Usuário autenticado e com acesso ao sistema.

Fluxo Principal:

O usuário abre o aplicativo

Informa login e senha

O sistema valida as credenciais

O sistema permite o acesso

Fluxos Alternativos:

2a. Senha incorreta → sistema exibe mensagem de erro

2b. Usuário não encontrado → acesso negado

3a. Falha de conexão → sistema informa erro

2. Caso de Uso: Cadastrar Produto

Ator: Usuário
Descrição: Permite cadastrar novos produtos (couve/milho).
Pré-condições: Usuário autenticado
Pós-condições: Produto registrado no sistema

Fluxo Principal:

Usuário acessa a tela de cadastro

Informa nome, tipo e quantidade inicial

Confirma cadastro

Sistema salva o produto

Fluxos Alternativos:

2a. Campos vazios → sistema solicita preenchimento

2b. Produto já cadastrado → sistema exibe alerta

3. Caso de Uso: Registrar Entrada de Estoque

Ator: Usuário
Descrição: Permite adicionar produtos ao estoque.
Pré-condições: Produto deve estar cadastrado
Pós-condições: Estoque atualizado

Fluxo Principal:

Usuário seleciona produto

Informa quantidade de entrada

Confirma operação

Sistema atualiza o estoque

Fluxos Alternativos:

2a. Quantidade inválida → operação bloqueada

1a. Produto não encontrado → erro exibido

4. Caso de Uso: Registrar Saída (Venda)

Ator: Usuário
Descrição: Permite registrar a venda de produtos.
Pré-condições: Produto disponível em estoque
Pós-condições: Estoque reduzido

Fluxo Principal:

Usuário seleciona produto

Informa quantidade vendida

Confirma operação

Sistema atualiza o estoque

Fluxos Alternativos:

2a. Quantidade maior que o estoque → operação negada

1a. Produto inexistente → erro exibido

5. Caso de Uso: Consultar Estoque

Ator: Usuário
Descrição: Permite visualizar o estoque atual.
Pré-condições: Usuário autenticado
Pós-condições: Nenhuma

Fluxo Principal:

Usuário acessa a tela de estoque

Sistema exibe lista de produtos e quantidades

Fluxos Alternativos:

2a. Nenhum produto cadastrado → sistema informa

6. Caso de Uso: Cadastrar Pedido

Ator: Usuário
Descrição: Permite registrar pedidos de clientes.
Pré-condições: Produtos cadastrados
Pós-condições: Pedido registrado

Fluxo Principal:

Usuário inicia novo pedido

Seleciona produtos e quantidades

Confirma pedido

Sistema salva o pedido

Fluxos Alternativos:

2a. Produto sem estoque → aviso exibido

3a. Dados incompletos → sistema impede cadastro

7. Caso de Uso: Gerenciar Entregas

Ator: Usuário
Descrição: Permite acompanhar e atualizar entregas.
Pré-condições: Pedido existente
Pós-condições: Status atualizado

Fluxo Principal:

Usuário seleciona pedido

Atualiza status (pendente, em entrega, entregue)

Sistema salva atualização

Fluxos Alternativos:

1a. Pedido não encontrado → erro exibido

8. Caso de Uso: Registrar Pagamento

Ator: Usuário
Descrição: Permite registrar pagamentos dos pedidos.
Pré-condições: Pedido existente
Pós-condições: Pagamento registrado

Fluxo Principal:

Usuário seleciona pedido

Informa valor e status do pagamento

Confirma registro

Sistema salva pagamento

Fluxos Alternativos:

1a. Pedido inexistente → erro exibido

9. Caso de Uso: Visualizar Dashboard

Ator: Usuário
Descrição: Permite visualizar indicadores do sistema.
Pré-condições: Dados cadastrados
Pós-condições: Nenhuma

Fluxo Principal:

Usuário acessa o dashboard

Sistema exibe:

Total de vendas

Produtos em estoque

Movimentações

Fluxos Alternativos:

2a. Sem dados → sistema exibe mensagem informativa
