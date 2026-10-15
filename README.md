# Porsche Sales Intelligence

Dashboard interativo para explorar registros de vendas de veículos Porsche por modelo, ano do modelo, cidade, método de pagamento e período.

**Acesse o dashboard:** [Dashboard Porsche Sales](https://eds-almeida.github.io/Dashboard_Porshe_sales/)

## Perguntas de negócio respondidas

Os resultados abaixo correspondem à base completa, com os filtros limpos:

| Pergunta | Resposta observada |
| --- | --- |
| Quantos registros de vendas estão na base? | **100 registros.** |
| Qual é o modelo mais vendido? | Há um empate: **Cayenne Coupe, Taycan 4S, Cayenne E-Hybrid, Panamera, Macan Electric e Macan T**, com **4 vendas cada** (4% do total por modelo). Não há um único modelo líder. |
| Qual ano de modelo aparece mais? | **2024**, com **29 veículos**. Esse campo representa o ano do modelo, não o ano da venda. |
| Em qual cidade houve mais vendas? | **Atlanta**, com **3 registros**. A base abrange **79 cidades**, portanto o volume está bastante distribuído e a liderança é pequena. |
| Qual método de pagamento foi mais utilizado? | **Wire Transfer**, com **26 registros**. |
| Qual combinação de modelo e ano teve maior saída? | **Macan T · 2022**, com **4 registros**. |
| Como interpretar a preferência por modelo em cada cidade? | O painel compara o modelo líder e sua participação nas vendas locais, sinalizando empates. Como os volumes por cidade são baixos, essas preferências devem ser tratadas como indicativas, não conclusivas. |

O painel também apresenta rankings de modelos, cidades, combinações de modelo e ano e formas de pagamento, além da evolução mensal e de uma tabela com até 100 registros correspondentes aos filtros.

## Como usar

- Filtre por **modelo**, **ano do modelo**, **cidade** ou **método de pagamento**.
- Use **Venda a partir de** e **Venda até** para restringir o período da venda.
- Os indicadores, rankings, insights e tabelas acompanham os filtros aplicados.
- Clique em **Limpar filtros** para retornar à visão completa.

## Dados e tratamento

O **ChatGPT foi utilizado no tratamento dos dados e na criação do dashboard**. A página é implementada em HTML, CSS e JavaScript, e os registros usados na visualização estão incorporados ao próprio dashboard.

## Observações sobre os dados

- A base contém **100 registros**, dos quais **24 têm data de venda inválida**. Esses registros continuam nas análises sem filtro de período; a série mensal não os considera e um filtro por período também os exclui.
- As datas válidas vão de **14/03/2024 a 01/10/2027**. Vale validar as datas posteriores a 2026 para confirmar se são registros esperados.
- Os valores de venda estão em **USD**, conforme a base. O painel mostra o valor nos registros, mas seus indicadores e rankings apresentados aqui são baseados em **quantidade de vendas**, não em receita, margem ou lucro.
- Empates no ranking não indicam preferência única. Cidades com poucas vendas exigem cautela ao interpretar percentuais locais.
