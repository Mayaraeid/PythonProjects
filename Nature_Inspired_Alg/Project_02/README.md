# Otimização por Colônia de Formigas para TSP 🐜🗺️

Este projeto implementa o algoritmo de **Otimização por Colônia de Formigas (ACO)** para resolver o clássico **Problema do Caixeiro Viajante (TSP)** utilizando dados de cidades de Berlim.

## 🧠 Sobre o Algoritmo

O algoritmo ACO é inspirado no comportamento das formigas que, coletivamente, são capazes de encontrar o caminho mais curto entre sua colônia e uma fonte de alimento. As formigas depositam feromônios ao longo do caminho, criando uma forma de "inteligência coletiva" que guia outras formigas para rotas mais eficientes.

## 🗺️ O Problema do Caixeiro Viajante

O TSP consiste em encontrar a rota mais curta que percorre todas as cidades exatamente uma vez e retorna à cidade de origem. Este é um problema NP-difícil, e métodos exatos são impraticáveis para um grande número de cidades.

## ⚙️ Detalhes da Implementação

O notebook realiza:

- **Carregamento de dados**: Lê coordenadas X e Y das cidades a partir do arquivo `DadosBerlim.xlsx`
- **Cálculo de distâncias**: Utiliza distância euclidiana entre todas as cidades
- **Inicialização**: Define posições iniciais aleatórias para as formigas
- **Processo iterativo**:
  - Construção probabilística de caminhos por cada formiga
  - Atualização de feromônios nos caminhos percorridos
  - Evaporação de feromônios ao longo do tempo
  - Aplicação de elitismo para reforçar os melhores caminhos encontrados
- **Visualização**: Mostra a evolução da busca e o melhor caminho final encontrado

## 📊 Parâmetros do Algoritmo

Os seguintes parâmetros foram utilizados na implementação:

- `alfa = 1`: Importância do feromônio na decisão do caminho
- `beta = 4`: Importância da heurística (distância) na decisão do caminho
- `rho = 0.2`: Taxa de evaporação do feromônio
- `num_formigas = 52`: Quantidade de formigas (mesma quantidade de cidades)
- `Q = 100`: Quantidade de feromônio depositado por cada formiga
- `b = 10`: Fator de elitismo
- `num_iteracoes = 50`: Número de gerações do algoritmo

## 📈 Visualizações

O projeto utiliza a biblioteca **matplotlib** para gerar dois gráficos essenciais:

1. **Gráfico de convergência**: Mostra a evolução da menor distância encontrada ao longo das iterações
2. **Visualização da rota**: Apresenta graficamente o melhor caminho encontrado pelo algoritmo, com as cidades como pontos e o trajeto como linhas que as conectam
