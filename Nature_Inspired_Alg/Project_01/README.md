# Classificação de Vinhos com Rede Neural 🍷🧠

Este projeto implementa uma **Rede Neural Artificial** para classificar tipos de vinhos baseado em suas propriedades químicas utilizando um conjunto de dados de análises de vinhos italianos.

## 🧪 Sobre o Conjunto de Dados

O conjunto de dados contém resultados de análises químicas de vinhos cultivados na mesma região da Itália, mas derivados de três cultivares diferentes. Cada amostra possui 13 atributos:

* **Álcool**
* **Ácido málico**
* **Cinzas**
* **Alcalinidade das cinzas**
* **Magnésio**
* **Fenóis totais**
* **Flavonoides**
* **Fenóis não flavonoides**
* **Proantocianidinas**
* **Intensidade de cor**
* **Matiz**
* **OD280/OD315**
* **Prolina**

A variável alvo é a identificação do tipo de vinho (classes 1, 2 e 3).

## 🧠 Arquitetura da Rede Neural

A rede neural implementada possui:

* **Camada de entrada**: 13 neurônios (um para cada característica)
* **Camada oculta**: 5 neurônios com ativação sigmoid
* **Camada de saída**: 3 neurônios (um para cada classe) com ativação softmax

## ⚙️ Detalhes da Implementação

O notebook realiza:

* **Carregamento de dados**: Lê o arquivo `DadosWine.xlsx`
* **Pré-processamento**: Normalização dos dados usando z-score
* **Divisão dos dados**: Separação em conjuntos de treino (70%), validação (20%) e teste (10%)
* **Inicialização da rede**: Usando inicialização de Xavier para os pesos
* **Treinamento**:
 * Propagação para frente (forward propagation)
 * Retropropagação (backpropagation)
 * Atualização de pesos
* **Avaliação**: Cálculo de acurácia e matrizes de confusão
* **Visualização**: Gráficos de evolução do treinamento

## 📊 Parâmetros do Modelo

Os seguintes parâmetros foram utilizados:

* `input_tam = 13`: Tamanho da camada de entrada (número de características)
* `hidden_tam = 5`: Tamanho da camada oculta
* `output_tam = 3`: Tamanho da camada de saída (número de classes)
* `taxa_aprendizado = 0.2`: Taxa de aprendizado para atualização de pesos
* `qtd_epoca = 1000`: Número de épocas de treinamento

## 📈 Visualizações

O projeto utiliza as bibliotecas **matplotlib** e **seaborn** para gerar visualizações importantes:

1. **Gráfico de acurácia**: Mostra a evolução das acurácias de treino, validação e teste ao longo das épocas
2. **Gráfico de erro médio quadrático**: Apresenta a evolução do MSE ao longo das épocas
3. **Matrizes de confusão**: Visualização das classificações corretas e incorretas para os conjuntos de treino, validação e teste usando seaborn para melhor representação visual por meio de mapas de calor

## 🎯 Resultados

A rede neural consegue classificar com sucesso os três tipos de vinho com alta precisão.

## 🛠️ Bibliotecas Utilizadas

* **NumPy**: Para operações numéricas
* **Pandas**: Para manipulação de dados
* **Matplotlib**: Para visualizações
* **Scikit-learn**: Para pré-processamento e métricas
* **Seaborn**: Para visualizações avançadas
* **PrettyTable**: Para exibição de tabelas formatadas

Este projeto demonstra a implementação de uma rede neural do zero, sem utilizar frameworks de deep learning como TensorFlow ou PyTorch, destacando os fundamentos teóricos e matemáticos por trás das redes neurais artificiais.
