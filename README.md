# Projeto de Análise de Dados com K-Means

Este projeto tem como objetivo demonstrar o uso do algoritmo K-Means para análise de dados em Python. O K-Means é um algoritmo de clusterização que agrupa dados semelhantes em grupos, chamados clusters. Neste projeto, usaremos o conjunto de dados do câncer de mama disponível no scikit-learn para aplicar o K-Means e avaliar a qualidade do agrupamento.

## Como Funciona

Neste projeto, realizamos as seguintes etapas:

1. **Carregamento dos Dados**: Utilizamos o conjunto de dados do câncer de mama do scikit-learn, que contém informações médicas sobre tumores. O conjunto de dados é carregado e dividido em duas partes principais: `x`, que contém os dados das características, e `y`, que contém os rótulos dos tumores (maligno ou benigno).

2. **Pré-Processamento dos Dados**: Para garantir que todas as características tenham a mesma escala e não influenciem desproporcionalmente o algoritmo K-Means, normalizamos os dados usando o Min-Max Scaler. Esse passo é importante para o bom desempenho do K-Means, pois ele é sensível à escala dos dados.

3. **Criação do Modelo K-Means**: Criamos um modelo de K-Means com 2 clusters, utilizando a classe `KMeans` do scikit-learn. O objetivo é agrupar os tumores em dois grupos distintos com base nas características médicas.

4. **Avaliação do Modelo**: Para avaliar o desempenho do modelo K-Means, realizamos as seguintes etapas:

    - Calculamos os centroides dos clusters resultantes do modelo, que representam os pontos médios dos grupos formados.
    
    - Prevemos os rótulos dos clusters para os dados originais e armazenamos esses rótulos na variável `rotulos_kmeans`.
    
    - Calculamos o número de acertos comparando os rótulos previstos pelo K-Means com os rótulos reais (maligno ou benigno) presentes em `y`.
    
    - Calculamos a taxa de acertos em relação ao total de dados, que é uma medida de quão bem o modelo K-Means se ajustou aos dados.
    
    - Calculamos a acurácia utilizando a função `accuracy_score` do scikit-learn, que nos fornece uma métrica adicional para avaliar a qualidade dos agrupamentos.

## Resultados

Os resultados do projeto incluem as seguintes informações:

- **Centroides dos Clusters**: São os pontos médios dos grupos formados pelo K-Means. Esses centroides podem ser úteis para interpretar as características médias de cada grupo.

- **Rótulos dos Clusters Previstos**: São os rótulos atribuídos pelo K-Means a cada amostra do conjunto de dados. Esses rótulos indicam a que grupo cada tumor foi associado.

- **Acurácia**: É uma medida de quão bem o modelo K-Means se ajustou aos dados, expressa como uma porcentagem. Quanto maior a acurácia, melhor o modelo está em agrupar os dados de acordo com os rótulos reais.

Este projeto demonstra o processo completo de aplicação do algoritmo K-Means a um conjunto de dados do mundo real e a avaliação da qualidade dos agrupamentos obtidos.

---

Esta é a continuação da documentação em Markdown. Certifique-se de personalizar o conteúdo e adicionar informações relevantes ao seu projeto, conforme necessário.
