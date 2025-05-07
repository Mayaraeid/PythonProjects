# 📊 Análise Avançada de Dados e Algoritmos Inteligentes

Este repositório contém uma coleção de projetos relacionados à análise de dados, visualização estatística, machine learning e algoritmos de otimização. Desenvolvido como parte de pesquisa acadêmica, este trabalho demonstra diversas técnicas computacionais aplicadas a problemas reais.

## 🧠 Projetos Incluídos

O repositório está organizado em quatro projetos principais:

### 1. [DataInfo](./DataInfo) - Análise Exploratória e Visualização de Dados

Projeto focado na exploração, sumarização e visualização de informações estatísticas de conjuntos de dados. Utiliza extensivamente as bibliotecas matplotlib e seaborn para gerar visualizações eficientes e claras para complementar uma defesa de doutorado.

**Recursos principais:**
- Análise exploratória de dados (EDA)
- Estatísticas descritivas (média, mediana, desvio padrão)
- Detecção de valores ausentes e anomalias
- Visualizações avançadas (histogramas, boxplots, heatmaps)

### 2. [WineClassifier](./WineClassifier) - Classificação de Vinhos com Rede Neural

Implementação de uma Rede Neural Artificial para classificar tipos de vinhos com base em suas propriedades químicas, utilizando um conjunto de dados de análises de vinhos italianos.

**Recursos principais:**
- Rede neural implementada do zero
- Arquitetura com camadas de entrada (13 neurônios), oculta (5 neurônios) e saída (3 neurônios)
- Pré-processamento e normalização de dados
- Visualização da evolução do treinamento e matrizes de confusão

### 3. [ACO_TSP](./ACO_TSP) - Otimização por Colônia de Formigas para TSP

Implementação do algoritmo de Otimização por Colônia de Formigas para resolver o Problema do Caixeiro Viajante, utilizando dados de cidades de Berlim.

**Recursos principais:**
- Algoritmo bio-inspirado para otimização combinatória
- Simulação de comportamento coletivo de formigas
- Visualização da convergência e da rota ótima encontrada
- Aplicação de elitismo para melhorar a busca

### 4. [TrueRMS](./TrueRMS) - Cálculo e Análise de Valor Eficaz Verdadeiro

Projeto focado na implementação e análise computacional do cálculo do valor eficaz verdadeiro (True RMS) de sinais elétricos, com visualizações para validar e interpretar resultados.

**Recursos principais:**
- Processamento de sinais elétricos
- Cálculo matemático do True RMS
- Comparação entre valores teóricos e calculados
- Visualização de sinais no domínio do tempo

## 🛠️ Tecnologias Utilizadas

Este repositório faz uso extensivo das seguintes tecnologias:

- **Python 3.8+**: Linguagem de programação principal
- **NumPy**: Operações numéricas e manipulação de arrays
- **Pandas**: Manipulação e análise de dados tabulares
- **Matplotlib**: Visualização de dados e criação de gráficos
- **Seaborn**: Visualizações estatísticas avançadas
- **Scikit-learn**: Ferramentas de pré-processamento e avaliação
- **PrettyTable**: Formatação de tabelas para exibição

## 📄 Estrutura do Repositório

```
.
├── DataInfo/
│   ├── README.md
│   └── DataInfo.ipynb
├── WineClassifier/
│   ├── README.md
│   ├── WineClassifier.ipynb
│   └── DadosWine.xlsx
├── ACO_TSP/
│   ├── README.md
│   ├── ACO_TSP.ipynb
│   └── DadosBerlim.xlsx
├── TrueRMS/
│   ├── README.md
│   └── TrueRMS.ipynb
└── README.md (este arquivo)
```

## 🚀 Como Usar

Cada pasta de projeto contém seu próprio README.md com instruções específicas. Em geral, para executar qualquer notebook:

1. Clone este repositório
2. Instale as dependências necessárias:
   ```
   pip install numpy pandas matplotlib seaborn scikit-learn prettytable
   ```
3. Navegue até a pasta do projeto desejado
4. Execute o notebook Jupyter correspondente

## 📚 Contexto Acadêmico

Este conjunto de projetos foi desenvolvido para apoiar pesquisa acadêmica na área de análise de dados e algoritmos inteligentes. As implementações fornecem tanto valor educacional quanto ferramentas práticas para análise e visualização de dados complexos.

## 👨‍💻 Autor

Desenvolvido por Mayara Eid, 2024.
