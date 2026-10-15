# Porsche | Sales Intelligence 🏎️

**Dashboard interativa de análise de vendas de veículos Porsche**, desenvolvida para transformar registros comerciais em indicadores e apoiar decisões por cidade, modelo, ano do veículo e período.

![Status](https://img.shields.io/badge/status-em%20desenvolvimento-d5001c) ![HTML](https://img.shields.io/badge/HTML5-dashboard-1a1c20) ![JavaScript](https://img.shields.io/badge/JavaScript-interatividade-1a1c20)

**Repositório:** [eds-almeida/Dashboard_Porshe_sales](https://github.com/eds-almeida/Dashboard_Porshe_sales)  
**Dashboard (GitHub Pages):** [Acessar endereço previsto](https://eds-almeida.github.io/Dashboard_Porshe_sales/) — **publicação ainda não confirmada; validar após habilitar o Pages.**

> **Nota de transparência:** esta documentação distingue o que foi observado no código público das etapas de preparação de dados e publicação que ainda precisam ser confirmadas. Ajuste os campos indicados antes da entrega.

## 1. Objetivo e contexto

O projeto busca identificar padrões de demanda e concentração de vendas de veículos Porsche em diferentes cidades, ajudando a compreender quais modelos e anos se destacam e como as vendas se comportam ao longo do tempo. A interface utiliza identidade visual escura, acentos vermelhos, cartões de indicadores e componentes responsivos.

## 2. Perguntas de negócio e justificativas

| Pergunta | Por que importa | Análise esperada |
|---|---|---|
| Quais são os modelos mais vendidos em cada cidade? | Apoia decisões de estoque e distribuição regional. | Ranking de modelos por cidade. |
| Qual combinação de modelo e ano do veículo teve mais vendas no período? | Identifica produtos com maior saída. | Ranking filtrado por período, modelo e ano. |
| Como o volume de vendas evoluiu ao longo do tempo? | Ajuda a identificar crescimento, queda e sazonalidade. | Comparação temporal de vendas. |
| Quais modelos são mais populares em cada mercado local? | Permite diferenciar estratégias comerciais por região. | Participação e concentração de modelos por cidade. |

**Atenção:** quantidade de registros de venda não equivale necessariamente a faturamento ou lucro. Não interpretar volume como receita sem uma coluna monetária válida.

## 3. Dashboard e experiência de uso

O arquivo público `index.html` contém HTML e CSS da interface, incluindo áreas de filtros, cartões de KPI, gráficos de barras, tabela, insights e campos de data. O layout prevê adaptação a telas menores. A presença desses componentes no código **não substitui o teste funcional no navegador**.

### Demonstração visual

**Captura da visão geral:**

> 📷 **Pendente:** adicionar `assets/dashboard-visao-geral.png` após capturar a dashboard funcionando.

**Exemplo com filtro aplicado:**

> 📷 **Pendente:** selecionar uma cidade e/ou período, confirmar a atualização dos indicadores e adicionar `assets/dashboard-filtro-aplicado.png`.

**Roteiro de validação:** abrir a página; registrar os valores iniciais; selecionar uma cidade; observar se rankings, tabela e KPIs mudam; alterar o intervalo de datas; testar a opção de limpar filtros; repetir em dispositivo móvel.

## 4. Indicadores e critérios de interpretação

- **Total de vendas:** contagem de transações ou soma da coluna de quantidade, conforme o esquema real da base.
- **Modelos líderes:** classificação por volume de vendas no recorte selecionado.
- **Distribuição geográfica:** comparação das vendas entre cidades.
- **Evolução temporal:** vendas agrupadas por período, quando houver datas válidas.
- **Ano do veículo:** distinguir ano/modelo do automóvel de ano em que a venda ocorreu.

Os valores e os resultados específicos devem ser conferidos na base e na dashboard antes de serem divulgados como conclusões.

## 5. Dados: origem, preparação e qualidade

**Origem:** planilha Excel usada na etapa de construção da dashboard. **O arquivo original não estava disponível no repositório público consultado**; por isso, o histórico exato de transformações ainda precisa ser documentado.

### Checklist de preparação (confirmar o que foi efetivamente realizado)

1. Conferir nomes e tipos das colunas (cidade, modelo, ano do veículo, data e quantidade, se disponíveis).
2. Padronizar nomes de cidades e modelos, removendo espaços extras e variações de escrita.
3. Validar datas, anos e valores numéricos; sinalizar registros inválidos.
4. Examinar dados ausentes, duplicados e registros inconsistentes.
5. Definir a unidade de análise: uma linha representa uma venda, um veículo ou uma agregação?
6. Conferir totais e rankings antes e depois da transformação.
7. Remover informações pessoais, identificadores sensíveis e dados não autorizados para publicação.
8. Preparar os dados para consumo pelo HTML/JavaScript, verificando se foram incorporados à página.

**Registrar antes da entrega:** número de linhas antes/depois, colunas usadas, exclusões, regras de duplicidade e exemplos de correções. Não declarar limpeza ou anonimização como concluídas sem evidência.

> ⚠️ **Privacidade:** se os registros estiverem embutidos no HTML, qualquer visitante poderá inspecioná-los. Publicar apenas dados autorizados e não sensíveis.

## 6. Inteligência artificial: prompt e evolução

**Ferramenta utilizada:** ChatGPT, em conversa para elaboração e refinamento da dashboard. **Não há evidência de uso do Canvas ou de um agente com skill específica**; portanto, não são declarados como utilizados.

### Prompt de negócio documentado

> “Responda as perguntas de negócio e KPIs: quais os principais modelos de carros vendidos por cidade; qual o ano e modelo de carro mais saiu em um período; quero insights de carros populares de vendas, com base em cada cidade. Sobre o UI/UX, se baseie no site oficial da Porsche.”

### Refinamento posterior registrado

> “Crie um gráfico de maneira evolutiva.”

**Evolução do pedido:** o escopo começou com rankings e comparações por cidade, modelo e ano; em seguida, passou a exigir uma apresentação visual alinhada à marca Porsche e uma visão de evolução temporal. O resultado foi estruturado como dashboard HTML com filtros, indicadores, áreas de visualização e insights.

**Importante:** os trechos acima registram as instruções de negócio conhecidas. Não representam necessariamente a transcrição integral de todas as mensagens usadas para gerar o código. A revisão humana deve validar fórmulas, filtros, contagens, tratamento dos dados e conclusões.

## 7. Tecnologias e arquitetura

- **HTML5:** estrutura da página.
- **CSS3:** identidade visual, componentes e responsividade.
- **JavaScript:** lógica de apresentação e interatividade, sujeita a validação funcional.
- **Excel:** formato da fonte de dados utilizada durante a análise.
- **GitHub Pages:** hospedagem estática pretendida.
- **ChatGPT:** apoio à geração e ao refinamento da dashboard.

A estrutura pública verificada é:

```text
Dashboard_Porshe_sales/
└── index.html
```

**Estrutura sugerida após completar a documentação (não presumir que já exista):**

```text
Dashboard_Porshe_sales/
├── index.html
├── README.md
└── assets/
    ├── dashboard-visao-geral.png
    └── dashboard-filtro-aplicado.png
```

## 8. Como executar

1. Acesse o repositório e obtenha o arquivo `index.html`.
2. Abra-o em um navegador moderno.
3. Confira se os dados, gráficos e filtros carregam corretamente.
4. Para disponibilizar a versão online, abra **Settings → Pages** no repositório, selecione **Deploy from a branch**, escolha a branch `main` e a pasta `/ (root)` e salve.
5. Aguarde a implantação e teste o endereço indicado no início deste documento.

**Observação:** o endereço do Pages é um endereço **previsto**, não uma comprovação de que a publicação esteja ativa.

## 9. Resultados e possibilidades de decisão

A dashboard foi concebida para apoiar a identificação de modelos líderes por cidade, a comparação de anos de veículo e a observação da evolução das vendas. Esses recortes podem orientar decisões sobre alocação de estoque, priorização comercial e acompanhamento de desempenho. **Resultados quantitativos concretos só devem ser apresentados depois de validar os dados e o funcionamento dos filtros.**

## 10. Limitações e próximos passos

- Documentar a origem e o tratamento efetivamente aplicado à planilha.
- Publicar e testar o GitHub Pages.
- Incluir duas capturas reais: visão geral e filtro aplicado.
- Validar cálculos e comportamento dos filtros em diferentes períodos.
- Avaliar completude, duplicidades, consistência, validade e atualidade dos registros.
- Melhorar a organização do repositório e considerar nome em minúsculas, sem acentos e com a grafia correta de **Porsche** (por exemplo, `dashboard-porsche-sales`). **Renomear altera os links**, que precisarão ser atualizados.

## 11. Checklist de entrega

- [x] Repositório público localizado no GitHub.
- [x] Arquivo `index.html` localizado no repositório.
- [ ] Adicionar este `README.md` ao repositório.
- [ ] Confirmar GitHub Pages acessível e funcionando.
- [ ] Validar filtros, KPIs e gráficos no navegador.
- [ ] Adicionar prints reais da visão geral e do filtro aplicado.
- [ ] Confirmar e documentar tratamento da base.
- [ ] Verificar ausência de dados sensíveis no HTML.
- [ ] Conferir todos os links e arquivos mencionados.
- [ ] Enviar **o link do repositório**, e não apenas o da dashboard.

---

**Projeto de portfólio — Análise de Dados, Business Intelligence e IA generativa.**  
**Autor:** Edson Luís de Almeida · [Perfil no GitHub](https://github.com/eds-almeida)

*Projeto independente para fins educacionais e de portfólio; não afiliado à Porsche AG.*
