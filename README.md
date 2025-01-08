# Clustering-CreditCard

## Introdução
  Este projeto utiliza o algoritmo de clustering K-Means para realizar a segmentação de clientes de cartões de crédito. O objetivo é agrupar clientes com base em padrões de comportamento, como compras realizadas e limites de crédito, fornecendo informações valiosas para personalização de serviços e campanhas de marketing.

## Benefícios da Segmentação

  O clustering de cartões de crédito auxilia empresas a: 
    Personalizar estratégias de marketing com base nos perfis dos clientes.
    Identificar clientes em potencial para vendas cruzadas ou up-selling.
    Otimizar campanhas e recursos com foco em grupos-alvo bem definidos.

## Métricas de Avaliação

  Foram utilizadas duas principais métricas para avaliar a qualidade dos clusters:
    Silhouette Score: Mede a coesão e separação dos clusters. Valores mais próximos de 1 indicam uma segmentação bem definida.
    Davies-Bouldin Index: Avalia a compacidade e separação dos clusters. Valores mais baixos são desejáveis.

## Resultados com 2 Clusters

  Silhouette Score: 0.5307 (indica boa separação e coesão).
  Davies-Bouldin Index: 0.9368 (mostra clusters compactos e bem separados).

## Estrutura do Arquivo Jupyter

O notebook está organizado nas seguintes etapas:

  1. Importação de Bibliotecas
      As bibliotecas utilizadas incluem:
       pandas para manipulação de dados.
       numpy para operações matemáticas.
       matplotlib e seaborn para visualizações.
       scikit-learn para aplicação do algoritmo de clustering e métricas de avaliação.

  2. Carregamento e Limpeza dos Dados
      Os dados brutos são carregados em um DataFrame.
      São realizadas transformações, como remoção de valores nulos e normalização das variáveis para garantir comparabilidade.

  3. Análise Exploratória dos Dados

      Visualizações gráficas, como histogramas e scatterplots, são utilizadas para entender distribuições e relações entre variáveis.

  4. Aplicando o Algoritmo de Clustering

      O algoritmo K-Means é aplicado com 5,3 e 2 clusters.
      As métricas de avaliação (Silhouette Score e Davies-Bouldin Index) são calculadas para validar a segmentação.

  5. Visualização dos Clusters
      Os clusters formados são visualizados em gráficos de dispersão, destacando as características "BALANCE", "PURCHASES" e "CREDIT_LIMIT".

  6. Interpretação dos Resultados

      Os clusters identificados representam perfis de clientes com comportamentos semelhantes, como:

        Cluster 1: Clientes com limites de crédito mais baixos e volume de compras menor.
        Cluster 2: Clientes com limites de crédito mais altos e volume de compras maior.
