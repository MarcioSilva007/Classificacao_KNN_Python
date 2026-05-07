# Classificacao_KNN_Python

Aqui está uma proposta de README estruturada e profissional para o seu GitHub, baseada no código e nas análises presentes no seu arquivo KNNimg.ipynb.

📝 Classificação de Dígitos com K-Nearest Neighbors (KNN)
Este projeto apresenta a implementação e otimização de um modelo de Machine Learning utilizando o algoritmo KNN (K-Nearest Neighbors) para o reconhecimento de dígitos manuscritos, utilizando o conjunto de dados Digits do scikit-learn.

🚀 Visão Geral do Projeto
O objetivo é classificar imagens de baixa resolução (8x8 pixels) em categorias de 0 a 9. O projeto cobre desde a análise exploratória e visualização dos dados até a normalização, ajuste de hiperparâmetros e validação final do modelo.

🛠️ Tecnologias Utilizadas
Python 3.x.

Scikit-Learn: Para carregamento do dataset, divisão de dados (train_test_split), métricas e o modelo KNN.

NumPy: Para manipulação de matrizes e cálculos de normalização.

Matplotlib & Seaborn: Para visualização de dados, exibição de imagens e plotagem da matriz de confusão.

📈 Etapas de Desenvolvimento
1. Exploração e Visualização
O dataset contém 1.797 amostras com 64 atributos cada. Foi realizada a visualização das primeiras amostras para entender a representação dos números em escala de cinza.

2. Pré-processamento e Divisão
Divisão de Dados: Os dados foram segmentados em Treino (1.131 amostras), Validação (126 amostras) e Teste (540 amostras).

Normalização: Foi aplicada a centralização dos dados subtraindo a média (X_norm) de todos os conjuntos para melhorar a eficiência do algoritmo de distância.

3. Otimização do Hiperparâmetro K
Foi realizado um teste iterativo com valores ímpares de K (de 1 a 30) para identificar qual oferecia a melhor acurácia no conjunto de validação.

Resultado: O valor K=5 obteve 100% de acurácia nos dados de validação.

4. Avaliação de Performance
O modelo final foi testado com dados inéditos (conjunto de teste), apresentando:

Acurácia Global: 98%.

Métricas detalhadas: Relatório de classificação com precision, recall e f1-score para cada dígito.

Análise de Erros: Matriz de Confusão visual (Heatmap) para identificar falsos positivos e negativos.

5. Predição em Novos Dados
O projeto inclui uma etapa de predição funcional, onde o modelo recebe um novo vetor de pixels, realiza a normalização e retorna a classe prevista.

Exemplo: Ao receber um novo dígito, o modelo previu corretamente a classe correspondente.

🏆 Resultados Finais
O modelo demonstrou alta robustez, mantendo uma precisão de 100% para os dígitos 0, 2 e 6, e mínima confusão em dígitos mais complexos como o 8.

📂 Como Executar
Clone este repositório.

Certifique-se de ter as bibliotecas instaladas: pip install scikit-learn numpy matplotlib seaborn.

Execute o notebook KNNimg.ipynb.
