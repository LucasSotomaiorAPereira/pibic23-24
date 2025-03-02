# Projeto de Classificação Musical com Machine Learning
A classificação musical desempenha um papel crucial na análise de dados e inteligência artificial, com aplicações em áreas como recomendação musical, organização de bibliotecas digitais e análise de tendências do mercado. Este projeto, desenvolvido como parte de uma pesquisa acadêmica, investiga o impacto das técnicas de balanceamento de dados na classificação de músicas tradicionais irlandesas, visando aprimorar a precisão dos modelos de aprendizado de máquina, especialmente na previsão de classes minoritárias.

## Metodologia

Este projeto utiliza um conjunto de dados de 10.200 músicas tradicionais irlandesas, classificadas em 11 gêneros distintos, cada uma representada por 1.022 características musicais de alto nível. Para mitigar o viés do desequilíbrio entre as classes, foram aplicadas técnicas de balanceamento de dados, incluindo SMOTE (Synthetic Minority Oversampling Technique) e Tomek Links.

**SMOTE:** SMOTE aborda o desequilíbrio de classes gerando amostras sintéticas da classe minoritária, aumentando sua representação no conjunto de dados.

**Tomek Links:** Tomek Links identifica e remove pares de amostras de classes diferentes que estão muito próximas, "limpando" a fronteira entre as classes.

Diversos algoritmos de classificação foram empregados, incluindo Decision Tree, Random Forest, Naive Bayes, Multilayer Perceptron e SVM, combinados com as estratégias de balanceamento e comparados usando validação cruzada em 10 partições. O desempenho foi avaliado por meio de métricas como acurácia, precisão, recall e F1-score, além da análise de matrizes de confusão.

## Resultados

Os resultados demonstram que a aplicação das técnicas de balanceamento de dados, especialmente SMOTE e Tomek Links, resultou em melhorias na performance dos classificadores, particularmente em relação à classe minoritária 'three_two'. O classificador Random Forest, combinado com SMOTE e k=3, alcançou o melhor desempenho em termos de F-measure, com 92,59% e um desvio padrão de 0.0074.

## Conclusões

Este estudo evidencia o impacto positivo das técnicas de balanceamento de dados na classificação musical, especialmente em conjuntos de dados desequilibrados. A escolha do algoritmo de classificação e da estratégia de balanceamento influencia significativamente o desempenho, e a combinação ideal varia de acordo com o conjunto de dados e as métricas de avaliação.

## Tecnologias Utilizadas

* Linguagem de Programação: Python
* Bibliotecas:
    * Pandas
    * Scikit-learn (sklearn)
    * Imbalanced-learn (imblearn)

## Próximos Passos

* Investigar o impacto de outras técnicas de balanceamento de dados, como Random Oversampling e Undersampling.
* Explorar a otimização de hiperparâmetros dos algoritmos de classificação para aprimorar ainda mais o desempenho.
* Avaliar a generalização dos modelos treinados em outros conjuntos de dados de música tradicional irlandesa.
