# Project TrueRMS 📊

Este projeto tem como objetivo a implementação e análise computacional do cálculo do valor eficaz verdadeiro (*True RMS*) de sinais elétricos, utilizando Python e bibliotecas de visualização para entender e validar os resultados de forma clara e interpretável.

## ⚙️ Descrição técnica

O valor eficaz (Root Mean Square, RMS) é uma métrica fundamental na engenharia elétrica, usada para quantificar a potência de sinais alternados. Em sinais arbitrários (não puramente senoidais), o cálculo do **True RMS** exige processamento de amostras discretas e integração numérica.

Este projeto:

- Lê e processa sinais de tensão e corrente (sintéticos ou reais).
- Aplica o cálculo matemático do True RMS diretamente sobre os dados amostrados.
- Compara o valor RMS real com valores obtidos por aproximações ou técnicas alternativas.
- Realiza a visualização dos sinais e dos resultados para facilitar a interpretação.

## 🖼️ Visualização com Matplotlib e Seaborn

As bibliotecas **matplotlib** e **seaborn** são centrais neste projeto. Elas permitem:

- 📉 Traçar os sinais de entrada no domínio do tempo com clareza e personalização.
- 📊 Gerar histogramas e gráficos de dispersão para explorar a distribuição dos dados.
- 🎯 Comparar graficamente os valores RMS esperados vs. calculados.
- 🎨 Usar temas, cores e estilos que destacam os padrões e tornam os gráficos publicáveis.

Essa camada visual é crucial para validar os resultados e comunicar a lógica do cálculo de forma didática e profissional.

## 🛠️ Tecnologias e bibliotecas utilizadas

- [Python 3.8+](https://www.python.org/)
- [NumPy](https://numpy.org/) – manipulação de arrays e operações matemáticas.
- [Matplotlib](https://matplotlib.org/) – gráficos técnicos e customizados.

## 🧪 Exemplos de visualização

O notebook inclui:

- Gráficos de linha para sinais de tensão e corrente.
- Histogramas da distribuição dos valores amostrados.
- Boxplots para analisar variabilidade e valores extremos.
- Comparações visuais entre métodos RMS aproximados vs. exato.
