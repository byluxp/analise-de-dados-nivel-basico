# Consultas SQL

- Uma consulta por arquivo, numerada: `01_total_de_pedidos.sql`, `02_receita_por_mes.sql`...
- Todo arquivo começa com um comentário dizendo **a pergunta** e **o que o resultado significa**:

```sql
-- Pergunta: ...
-- Resultado: ... (com unidade: pedidos, R$, itens)
```

- Validações (contagens antes/depois de JOIN, totais conferidos de outro jeito) vão em `validacao.md`.

## Como rodar
Com o [DuckDB](https://duckdb.org/), dá para consultar os CSVs direto, sem montar banco:

```sql
SELECT COUNT(*) FROM 'data/raw/olist_orders_dataset.csv';
```
