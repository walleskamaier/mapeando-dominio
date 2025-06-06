# mapeando-dominio
Atividade do MBA, módulo de backend.


## Entidades de Domínio ##
- Produto
Atributos: ID único, nome, tamanho, cor, quantidade atual, quantidade mínima, preço
Representa os itens físicos do estoque

- Movimentação de Estoque
Atributos: data, tipo (entrada/saída), quantidade, produto relacionado
Registra todas as alterações no estoque

- Venda
Atributos: data, produto, quantidade vendida, valor, lucro
Representa as transações de venda realizadas

- Alerta
Atributos: tipo, mensagem, data de criação, produto relacionado, status
Notificações sobre estoque baixo

- Ordem de Compra
Atributos: data de criação, fornecedor, produtos solicitados, quantidades, status, prazo de entrega
Pedidos feitos aos fornecedores

- Fornecedor
Atributos: nome, contato, produtos fornecidos, prazos de entrega
Empresas que fornecem produtos

## Casos de Uso (Ações) ##
- Gestão de Produtos
Cadastrar produto com ID único
Adicionar informações complementares (tamanho, cor)
Definir quantidade mínima de estoque
Atualizar informações do produto

- Controle de Estoque
Registrar entrada de produtos
Registrar saída de produtos
Consultar quantidade atual
Rastrear movimentações individuais

- Sistema de Alertas
Monitorar níveis de estoque
Gerar alertas de estoque baixo
Enviar notificações por e-mail
Exibir alertas no sistema

- Relatórios e Análises
Visualizar histórico de vendas por período
Calcular lucro por produto
Identificar produtos mais vendidos
Analisar tendências de estoque ao longo do tempo
Gerar relatórios de performance

- Gestão de Compras
Criar ordens de compra automaticamente
Gerenciar ordens de compra existentes
Integrar com fornecedores
Receber atualizações de prazos de entrega
Tomar decisões de compra baseadas em tendências
