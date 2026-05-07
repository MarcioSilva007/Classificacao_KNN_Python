# 📝 Classificação de Dígitos com K-Nearest Neighbors (KNN)

Este projeto apresenta a implementação e otimização de um modelo de Machine Learning utilizando o algoritmo **KNN (K-Nearest Neighbors)** para o reconhecimento de dígitos manuscritos, utilizando o conjunto de dados **Digits** do scikit-learn.

---

## 🚀 Visão Geral do Projeto
O objetivo é classificar imagens de baixa resolução (8x8 pixels) em categorias de 0 a 9.  
O projeto cobre desde a análise exploratória e visualização dos dados até a normalização, ajuste de hiperparâmetros e validação final do modelo.

---

## 🛠️ Tecnologias Utilizadas
- **Python 3.x**
- **Scikit-Learn**: carregamento do dataset, divisão de dados (`train_test_split`), métricas e modelo KNN
- **NumPy**: manipulação de matrizes e cálculos de normalização
- **Matplotlib & Seaborn**: visualização de dados, exibição de imagens e matriz de confusão

---

## 📈 Etapas de Desenvolvimento

### 🔍 Exploração e Visualização
- Dataset com **1.797 amostras** e **64 atributos** cada.  
- Visualização inicial das amostras para entender a representação dos números em escala de cinza.

### ⚙️ Pré-processamento e Divisão
- Divisão em **Treino (1.131 amostras)**, **Validação (126 amostras)** e **Teste (540 amostras)**.  
- Normalização: centralização dos dados subtraindo a média (`X_norm`) para melhorar a eficiência do algoritmo.

### 🔧 Otimização do Hiperparâmetro K
- Teste iterativo com valores ímpares de K (1 a 30).  
- **Resultado:** K=5 obteve **100% de acurácia** nos dados de validação.

### 📊 Avaliação de Performance
- Teste com dados inéditos (conjunto de teste).  
- **Acurácia Global:** 98%  
- Relatório de classificação com *precision*, *recall* e *f1-score*.  
- Matriz de Confusão visual (Heatmap) para análise de erros.

### 🤖 Predição em Novos Dados
- Modelo recebe vetor de pixels, normaliza e retorna a classe prevista.  
- Exemplo: ao receber um novo dígito, o modelo previu corretamente a classe correspondente.

---

## 🏆 Resultados Finais
- Alta robustez, com **100% de precisão** para os dígitos 0, 2 e 6.  
- Mínima confusão em dígitos mais complexos como o 8.

---

## 📂 Como Executar
1. Clone este repositório:
   ```bash
   git clone https://github.com/MarcioSilva007/Classificacao_KNN_Python.git
