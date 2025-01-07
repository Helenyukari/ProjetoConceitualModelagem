Descrição do Projeto Conceitual

O projeto visa desenvolver uma plataforma de e-commerce que permite a venda de produtos de diferentes fornecedores para consumidores finais. 
O sistema deve gerenciar informações sobre clientes, produtos, pedidos, pagamentos e logística de entrega, proporcionando uma experiência de compra eficiente e intuitiva.
Foi utilizado MYSQL para a modelagem de dados.


###Entidades Principais
Cliente: Representa os usuários do sistema que realizam compras. Inclui informações pessoais e de contato.
Produto: Representa os itens à venda, incluindo detalhes como descrição, categoria e preço.
Pedido: Registro das compras realizadas, incluindo detalhes de produtos adquiridos, valores e informações de pagamento.
Pagamento: Processamento das transações financeiras associadas aos pedidos.
Fornecedor: Entidades que disponibilizam produtos na plataforma.
Estoque: Informações sobre a disponibilidade física dos produtos.

###Relacionamentos
Os relacionamentos entre as entidades permitem que o sistema opere de maneira integrada:

Cada Cliente pode ter vários Pedidos.
Cada Pedido pode incluir múltiplos Produtos.
Pagamentos estão associados a um único Pedido.
Cada Produto pode ser fornecido por diferentes Fornecedores.
O Estoque controla a quantidade disponível de cada produto.

Cliente e Pedido: Um cliente pode fazer muitos pedidos (1:N).
Pedido e Carteira: Um pedido pode ter uma única carteira relacionada (N:1).
Pedido e Pagamento: Um pedido pode ter um pagamento associado (1:1).
Pagamento e Entrega: Um pagamento pode estar associado a uma entrega (1:1).
Pedido e Relação de Produto por Pedido: Um pedido pode envolver múltiplos produtos (1:N).
Produto e Relação de Produto por Pedido: Um produto pode estar incluso em vários pedidos (1:N).
Terceiro Vendedor e Produtos por Vendedor: Um vendedor pode oferecer muitos produtos (1:N).
Produto e Produtos por Vendedor: Um produto pode ser oferecido por vários vendedores (N:1).
Forneceder e Disponibilizando: Um fornecedor pode ter múltiplos produtos (1:N).
Produto e Disponibilizando: Um produto pode estar associado a vários fornecedores (N:M).
Estoque e Disponibilizando: Um estoque pode ter produtos disponíveis (1:N).
Produto e Estoque: Um produto pode estar disponível em vários locais (N:M).
