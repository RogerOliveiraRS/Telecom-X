![Capa do Repositório](https://github.com/RogerOliveiraRS/Telecom-X/blob/main/imagens/celular-telefonia-movel-espectro-radiofrequencia-freepik-768x492.jpg?raw=true)



# Análise de Churn de Clientes da TelecomX


---

## <span style="color: orange;">🚀 A Jornada de Descoberta por Trás da Desistência de Clientes</span>

A TelecomX é uma empresa de telecomunicações que enfrenta um desafio comum no setor: a perda de clientes, ou "churn". Cada cancelamento representa não apenas uma receita perdida, mas também uma oportunidade de melhorar a experiência do cliente. Por meio dessa análise, buscamos entender os padrões e fatores que levam os clientes a desistir e, assim, desenvolver estratégias eficazes de retenção.

### Metodologia  
Para alcançar esse objetivo, seguimos as seguintes etapas:
- **Coleta e Normalização dos Dados**: Os dados utilizados vêm da **base de clientes da TelecomX**, armazenados inicialmente em **formato JSON**.  
- **Limpeza e Preparação**: Tratamos valores nulos, removemos duplicatas e estruturamos os dados em um formato tabular para facilitar a análise.  
- **Segmentação e Visualização**: Agrupamos clientes por tipo de contrato, idade, serviços utilizados e forma de pagamento.  
- **Interpretação e Estratégias**: Geramos insights sobre os fatores de maior impacto no churn e propomos soluções para melhorar a retenção.  

### Tipos de Gráficos Utilizados  
Utilizamos diferentes tipos de gráficos para apresentar os padrões encontrados:
- **Gráficos de Pizza** → Comparação da taxa de churn entre diferentes categorias.  
- **Gráficos de Barras** → Visualização das diferenças nas taxas de churn por tipo de contrato e serviços utilizados.  
- **Histogramas** → Distribuição do tempo de permanência dos clientes antes do cancelamento.  
- **Gráficos de Dispersão** → Relação entre valores pagos mensalmente e tempo de contrato para identificar faixas de alto churn.  
- **Heatmaps** → Correlação entre diferentes serviços e sua influência na taxa de desistência.  
- **Gráficos de Regressão** → Tendências de churn no seguimento 65+ e no seguimento <65.  

Fonte dos Dados:  
Os dados analisados são provenientes da **base de clientes da TelecomX**, simulada a partir de padrões reais do setor de telecomunicações.  

---

## <span style="color: orange;">🎯 Nosso Objetivo: Entender e Combater o Churn</span>
O principal objetivo desta análise é identificar os principais motivadores por trás do churn de clientes na TelecomX. Ao entender "quem" está saindo e "por quê", podemos direcionar esforços de retenção de forma mais eficaz e construir um relacionamento mais sólido com nossos clientes.

---

## <span style="color: orange;">🛠️ A Caixa de Ferramentas: Limpeza e Preparação dos Dados</span>
Nossa jornada começou com os dados brutos da TelecomX, armazenados em um arquivo JSON. Para transformá-los em informações acionáveis, realizamos as seguintes etapas:

1. **Carregamento e Normalização:** Importamos os dados e os normalizamos para uma estrutura tabular mais fácil de trabalhar.
2. **Inspeção Inicial:** Verificamos a estrutura dos dados, os tipos de colunas e a presença de valores nulos.
3. **Limpeza Profunda:** Removemos dados duplicados e tratamos valores nulos para garantir qualidade na análise.
4. **Entendendo as Variáveis:** Exploramos os valores únicos das colunas categóricas mais relevantes.

---

## <span style="color: orange;">📊 Execução da Análise: Explorando os Fatores de Churn</span>

Após a preparação dos dados, iniciamos a análise exploratória para entender **quais fatores influenciam a taxa de desistência dos clientes**. Abaixo, cada etapa é acompanhada dos gráficos gerados.

---

### <span style="color: orange;">📈 Distribuição do Tempo de Contrato</span>

A análise da duração dos contratos revelou padrões importantes sobre **quando os clientes tendem a cancelar**. A maioria dos cancelamentos ocorre nos primeiros meses, com uma estabilização após esse período.

![Distribuição do Tempo de Contrato](https://github.com/RogerOliveiraRS/Telecom-X/blob/main/imagens_graficos/grafico_histograma_distrib_tempo_contrato_clientes.png)

Para aprofundar a relação entre **tempo de contrato e desistência**, comparamos a distribuição entre clientes que cancelaram e os que permaneceram ativos:

![Cancelados vs Não Cancelados](https://github.com/RogerOliveiraRS/Telecom-X/blob/main/imagens_graficos/grafico_histog_2linhas_Cancelados_vs_noCancelados.png)

---

### <span style="color: orange;">📊 Contratos e Taxa de Churn</span>

A relação entre **tipo de contrato e churn** mostra que **contratos mensais possuem a maior taxa de desistência**, enquanto contratos mais longos resultam em maior retenção.

![Percentual de Desistência por Tipo de Contrato](https://github.com/RogerOliveiraRS/Telecom-X/blob/main/imagens_graficos/grafico_barras_Percentual_Desist%C3%AAncia_vs_Tipo_Contrato.png)

Para investigar a influência das cobranças mensais, analisamos **a relação entre tempo de contrato e contas mensais**:

![Scatterplot Tempo de Contrato vs Contas Mensais](https://github.com/RogerOliveiraRS/Telecom-X/blob/main/imagens_graficos/grafico_scatter_Tempo_Contrato_Contas%20mensais_vs_Desistencia.png)

---

### <span style="color: orange;">🧑‍🤝‍🧑 Perfil Demográfico e Churn</span>

Exploramos como **gênero e idade** influenciam na taxa de churn. Descobrimos que **não há diferença significativa entre homens e mulheres** na desistência.

![Desistência por Gênero](https://github.com/RogerOliveiraRS/Telecom-X/blob/main/imagens_graficos/grafico_pizza_Desist_por_genero.png)

Já a **senioridade (65+) se mostrou um fator relevante**. Clientes mais velhos têm maior propensão ao cancelamento, como visto na análise comparativa:

![Desistência por Idade](https://github.com/RogerOliveiraRS/Telecom-X/blob/main/imagens_graficos/grafico_2%20pizzas_desist%C3%AAncia_%2065%2B_vs_jovens.png)

Para reforçar essa análise, utilizamos um **gráfico de regressão** mostrando a relação entre senioridade e taxa de desistência:

![Regressão Senioridade](https://github.com/RogerOliveiraRS/Telecom-X/blob/main/imagens_graficos/grafico_regress%C3%A3o_senioridade.png)

---

### <span style="color: orange;">💼 Serviços Contratados e Retenção</span>

A análise dos serviços mostrou que **certos serviços aumentam a retenção, enquanto outros têm menor impacto**. O **heatmap** abaixo ilustra a relação entre serviços contratados e taxa de churn:

![Taxa de Desistência por Serviço](https://github.com/RogerOliveiraRS/Telecom-X/blob/main/imagens_graficos/grafico_heatmap_tx_de_desistencia_vs_servico_oferecido.png)

---

### <span style="color: orange;">💳 Métodos de Pagamento e Fidelização</span>

Os métodos de pagamento também influenciam na retenção dos clientes. Identificamos que **clientes com contratos mais curtos tendem a evitar pagamentos automáticos**, enquanto **contratos mais longos têm maior uso de cartão de crédito ou transferência bancária**.

![Distribuição do Método de Pagamento vs Tempo de Contrato](https://github.com/RogerOliveiraRS/Telecom-X/blob/main/imagens_graficos/Grafico_barras_Distrib_Perc_M%C3%A9todo_pgto_vs_tempo_contrato.png)

---


## <span style="color: orange;">💡 Insights Chave e Recomendações Estratégicas</span>

Nossa análise revelou vários insights importantes para a TelecomX:
- **Focar na retenção inicial:** Melhorar a experiência nos primeiros meses pode reduzir a desistência.
- **Criar estratégias para clientes 65+:** Essa faixa etária tem taxas mais altas de churn e pode se beneficiar de um atendimento mais personalizado, visto que há picos de desistência antes dos períodos de vencimento dos contratos.
- **Aprimorar a experiência com Fibra Óptica e Paperless Billing:** Avaliar possíveis problemas nesses serviços e oferecer suporte melhor.
- **Destacar serviços de segurança e suporte técnico:** Clientes com esses serviços tendem a permanecer por mais tempo.
- **Reavaliar preços e benefícios para clientes de alto consumo:** Ajustes na precificação podem melhorar a retenção.

---

## <span style="color: orange;">📊 Próximos Passos</span>
- **Modelagem de Dados:** Incluir as datas do Início do contrato e do Churn.
- **Analisar:** satisfação e feedback dos clientes para ajustes estratégicos.
- **Análise preditiva:** Criar modelos de machine learning para prever clientes com maior probabilidade de churn.
- **Análise de custo-benefício:** Avaliar o impacto financeiro das estratégias de retenção propostas.
- **Testes A/B:** Implementar e testar diferentes iniciativas de retenção com grupos específicos de clientes.

---

## <span style="color: orange;">🔚 Conclusão</span>
Ao aplicar esses insights e continuar explorando os dados, a TelecomX pode transformar o desafio do churn em uma oportunidade para construir relacionamentos duradouros com seus clientes.


