# 📊 Projeto SQL – Análise de Vendas com Contoso

Este projeto foi realizado como parte da minha rotina de estudos e prática com SQL, utilizando o banco de dados **ContosoRetailDW**. O objetivo foi aplicar comandos essenciais para análise de dados:

## 🎯 Desafio
- Identificar os produtos mais vendidos com base na tabela `FactSales`, unindo com `DimProduct` para obter os nomes dos produtos.

## 🧠 Comandos Utilizados
- `JOIN`: combinação das tabelas `FactSales` e `DimProduct` pela chave `ProductKey`.
- `SUM()`: soma do valor de vendas (`SalesAmount`).
- `GROUP BY`: agrupamento dos dados por produto.
- `ORDER BY DESC`: ordenação do maior para o menor valor vendido.

## 📈 Resultado
- Produto mais vendido: **Proseware Projector 1080p DLP86 White**
- Valor total: **R$ 51.901.056,27**

## 💡 Código SQL Utilizado

```sql
SELECT 
    p.ProductName AS Produto,
    SUM(s.SalesAmount) AS Total_Vendido
FROM 
    FactSales s
JOIN 
    DimProduct p ON s.ProductKey = p.ProductKey
GROUP BY 
    p.ProductName
ORDER BY 
    Total_Vendido DESC;
```

## 📌 Prints do Projeto
Incluí uma captura de tela com a consulta executada e o resultado direto do SQL Server Management Studio (SSMS).

## 👨‍💻 Sobre mim
Me chamo **Paulo Claudio**, e estou em transição de carreira para a área de Dados e BI. Neste repositório você encontrará registros da minha evolução com SQL, Power BI, Python, Excel e análise de processos.

---

**LinkedIn:** [Clique aqui](https://www.linkedin.com/in/paulo-claudio-claudino-junior-1914ba183)  
**GitHub:** [Clique aqui](https://github.com/Paulodados-0411)
# sql-vendas-contoso
alem de treinar power bi é necessario treinar SQL tambem.
