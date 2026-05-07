# Classificacao_KNN_Python

📝 Classificação de Dígitos Escritos à Mão com KNN
Este projeto utiliza o algoritmo K-Nearest Neighbors (K-Neighbors Classifier) para reconhecer e classificar imagens de dígitos escritos à mão (0-9). O modelo foi desenvolvido em Python, utilizando a biblioteca scikit-learn e o famoso dataset Digits.

🚀 Visão Geral
O objetivo principal é demonstrar o fluxo de um projeto de Machine Learning, passando pela análise exploratória, pré-processamento (normalização), divisão de dados, otimização de hiperparâmetros (K) e avaliação de performance com métricas reais.

📊 O Dataset
O dataset contém 1.797 amostras de imagens 8x8 de dígitos. Cada pixel é um atributo (totalizando 64 atributos por imagem) com valores de intensidade de 0 a 16.

🛠️ Tecnologias Utilizadas
Python 3

Scikit-Learn: Criação do modelo, métricas e divisão de dados.

NumPy: Manipulação matemática e normalização.

Matplotlib/Seaborn: Visualização de dados e matriz de confusão.

Jupyter Notebook: Ambiente de desenvolvimento.

📈 Etapas do Projeto
Exploração: Visualização das matrizes de pixels como imagens.

Preparação:

Divisão em Treino (70%), Validação (10%) e Teste (20%).

Normalização dos dados subtraindo a média (Centralização).

Otimização: Execução de um loop para encontrar o melhor valor de K.

Resultado: O valor K=5 atingiu a maior acurácia nos dados de validação.

Avaliação:

Uso de Matriz de Confusão para identificar onde o modelo confunde números (ex: 8 com 1).

Geração de Relatório de Classificação (Precision, Recall, F1-Score).

🏆 Resultados
O modelo final alcançou uma performance excelente nos dados de teste:

Acurácia Global: ~98%

Melhor K: 5

Destaque: O modelo demonstrou alta precisão para quase todos os dígitos, com uma leve dificuldade em distinguir o dígito '8' de outros similares em casos específicos.

🖼️ Exemplo de Previsão
O notebook inclui uma seção de testes com imagens aleatórias do conjunto de teste, onde o modelo exibe o dígito e sua "crença" (predição):

Python
# Exemplo de saída do modelo
Eu acredito que esse seja: 5
📂 Como executar
Clone o repositório: git clone https://github.com/seu-usuario/nome-do-repo.git

Instale as dependências: pip install -r requirements.txt

Abra o arquivo KNNimg.ipynb em seu ambiente Jupyter.

⭐ Se este projeto te ajudou, sinta-se à vontade para dar uma estrela!
