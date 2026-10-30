# Dados

Os CSVs não são versionados (ver `.gitignore`).

## Como obter
1. Baixe o dataset em https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce (precisa de conta no Kaggle).
2. Descompacte os arquivos `.csv` em `data/raw/`.
3. Confira a licença na página do dataset e registre aqui se algo mudar.

## Tabelas usadas no projeto

| Arquivo | Uma linha é... | Campos principais |
|---|---|---|
| `olist_orders_dataset.csv` | um **pedido** | order_id, customer_id, order_status, order_purchase_timestamp |
| `olist_order_items_dataset.csv` | um **item de um pedido** | order_id, order_item_id, product_id, price, freight_value |
| `olist_products_dataset.csv` | um **produto** | product_id, product_category_name |
| `olist_customers_dataset.csv` | um **cliente por pedido** | customer_id, customer_unique_id, customer_state |
| `product_category_name_translation.csv` | uma **categoria** | nome em português e em inglês |

> Atenção à granularidade: a tabela de itens não tem coluna de quantidade. Cada linha é uma unidade vendida, e um pedido pode ter várias linhas.
