Este projeto demonstra como aplicar técnicas de ETL e EDA para entender melhor a evasão de clientes da Telecom X e descobrir insights relevantes para tomada de decisões estratégicas.

1. Análise de Evasão de Clientes (Churn) — Telecom X
Este projeto realiza uma análise detalhada sobre a evasão de clientes (churn) da Telecom X, utilizando técnicas de ETL (Extração, Transformação e Carga) e Análise Exploratória de Dados (EDA).

2. Tecnologias Utilizadas
- Python 3.x
- Pandas
- NumPy
- Seaborn
- Matplotlib
- JSON

3. Etapas do Projeto

3.1. Extração
Os dados foram extraídos de um arquivo JSON contendo informações estruturadas em formato aninhado. A extração foi realizada com a função json_normalize da biblioteca pandas.

3.2. Transformação
As transformações aplicadas incluíram:
- Padronização de nomes de colunas: remoção de prefixos como customer., internet., phone., account. e substituição de Charges. por Charges_.
- Conversão de tipos de dados: conversão de colunas como Charges_Total para float e tratamento de valores nulos.
- Normalização de categorias: categorias como 'No internet service' e 'No phone service' foram transformadas em 'No'.
- Codificação binária: variáveis como 'SeniorCitizen', 'Partner', 'Dependents' e outras foram convertidas para 0 e 1.

3.3. Carga
Após o processo de transformação, os dados foram carregados em um novo DataFrame (df_final) para realização da análise exploratória.Foi feito Carga e Análise (EDA) para:
- Distribuição de Churn:
- Churn por Tipo de Contrato:
- Churn por Método de Pagamento:
- Distribuição de Tenure por Churn:
- Churn por Tipo de Internet:
- Boxplot de Gastos Totais por Churn:
- Mapa de Calor de Correlação com Churn:

4. Análise Exploratória de Dados (EDA)
A taxa de churn foi calculada e os principais Insights encontrados foram:
- Clientes com contratos mensais tendem a ter maior taxa de churn.
- Formas de pagamento automáticas estão associadas a menor evasão.
- Quanto maior o tempo de permanência (tenure), menor a chance de churn.
- Serviços de internet também impactam diretamente a taxa de cancelamento.

5. Conclusões Parciais
- O tipo de contrato e o método de pagamento influenciam significativamente o churn.
- O tempo de permanência do cliente é um forte indicador de evasão.
- Serviços adicionais como segurança online e backup também apresentam correlação.  

