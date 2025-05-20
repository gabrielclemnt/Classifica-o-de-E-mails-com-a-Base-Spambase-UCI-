
# Classificação de E-mails com a Base Spambase (UCI)

Este projeto utiliza a base de dados Spambase do UCI Machine Learning Repository para construir e comparar modelos de classificação de e-mails em spam e não spam. O projeto foi desenvolvido no Google Colab, com o uso da biblioteca Scikit-learn.

📊 Objetivo
Aplicar e comparar o desempenho de quatro algoritmos de classificação:

Árvore de Decisão

Naive Bayes (Bayesiano Ingênuo)

Regressão Logística

K-Vizinhos mais próximos (KNN) com distância Euclidiana

🧪 Metodologia
Divisão dos dados: Estratificada e aleatória, com 70% dos dados para treinamento + validação e 30% para teste.

Validação de hiperparâmetros:

Modelos com hiperparâmetros foram ajustados via validação cruzada apenas no conjunto de treino/validação.

O conjunto de teste foi utilizado somente para avaliação final dos modelos.

Métricas de avaliação:

Precisão (Precision)

Cobertura (Recall)

F1-Score

📈 Curvas de Aprendizado
Para cada classificador com sua melhor configuração de hiperparâmetros, foram geradas curvas de aprendizado, variando a proporção de dados de treinamento de 5% até 95% (com passo de 5%). As métricas de avaliação foram plotadas em função do tamanho do conjunto de treinamento. Isso permite analisar o comportamento dos modelos conforme o volume de dados disponíveis.

🔧 Ferramentas Utilizadas
Google Colab

Scikit-learn

Matplotlib

Pandas

NumPy

📂 Organização do Projeto
spambase_classification.ipynb — Notebook principal com a implementação completa.

spambase.data — Dados originais da base (disponível via UCI ou repositório local).

README.md — Este arquivo.

📌 Resultados
Os modelos foram comparados com base em suas métricas no conjunto de teste. Também foi feita uma análise das curvas de aprendizado para cada algoritmo. Os melhores resultados variaram de acordo com as métricas, sendo o KNN e a Regressão Logística os modelos com desempenho mais consistente.

Este projeto mostrou a importância da validação de hiperparâmetros e da análise de curvas de aprendizado na construção de modelos robustos. Além disso, reforça a relevância do particionamento correto dos dados para evitar overfitting ou viés de avaliação.

