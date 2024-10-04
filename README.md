# Análise do Impacto do Trabalho Remoto na Saúde Mental

Este projeto apresenta o tratamento e limpeza de dados da base intitulada "impactos do trabalho remoto na saúde mental" disponibilizado pelo site kaggle e uma pequena análise utilizando as biblioteca `pandas` para manipulação de dados e `matplotlib` para visualização.

## Estrutura do Código

1. **Importação de Bibliotecas**
   ```python
   import pandas as pd
   import matplotlib.pyplot as plt
   ```

2. **Carregamento e Visualização dos Dados**
   - O conjunto de dados é carregado a partir do arquivo CSV chamado `Impact_of_Remote_Work_on_Mental_Health.csv`, traduzido como "impactos do trabalho remoto na saúde mental".
   - As primeiras linhas do dataframe são exibidas com `df.head()`.
   - Informações descritivas e a estrutura do dataframe são mostradas usando `df.describe()` e `df.info()`.

3. **Pré-processamento dos Dados**
   - Filtramos somente as colunas que achamos necessárias para nossa analise e removemos o restante:
     ```python
     df = df.drop(['Job_Role', 'Years_of_Experience', 'Company_Support_for_Remote_Work', 'Physical_Activity', 'Region'], axis=1)
     ```
   - Salvamos a base final tratada em um novo arquivo CSV chamado `Dados_SaudeMental.csv`.

4. **Análise Visual dos Dados**
   - **Análise quantitiva das Modalidades de Trabalho**
     - Um gráfico de barras é gerado para mostrar a distribuição das modalidades de trabalho, onde foi concluido que mais da metade da base trabalha de forma remota ou hibrida.

   - **Análise quantitativa do Nível de Estresse entre os colaboradores presente na base**
     - Um gráfico de barras é gerado para mostrar a distribuição dos níveis de estresse entre os colaboradores, onde foi concluido que a maioria dos colaboradores estão com nivel de estresse alto.

   - **Análise quantitativa da Saúde Mental dos colaboradores presentes na base**
     - Um gráfico de barras é gerado para mostrar a condição de saúde mental dos colaboradores, onde foi concluido que a maioria dos colaboradores está dividida em burnout e ansiedade.

5. **Observações Finais**
   - O código inclui impressões que resumem as descobertas principais, como a prevalência do trabalho remoto e os altos níveis de estresse e condições de saúde mental como burnout e ansiedade, a partir disso, faremos uma análise estudando a relação da saúde mental desses colaboradores com a modalidade a qual eles trabalham.



