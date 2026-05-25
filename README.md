# Predição da Resistência à Compressão do Concreto

Projeto de regressão aplicado à previsão da resistência à compressão do concreto com base em características dos materiais e do processo de cura. O trabalho combina análise exploratória de dados, engenharia de atributos e modelagem preditiva para estimar uma variável contínua de interesse em contexto de engenharia e ciência de dados.

<div align="center">
  <img src="./assets/grafico 3.png" alt="tip" width="800" />
</div>

## Sobre o projeto

Este projeto utiliza uma base com variáveis relacionadas à composição do concreto, como cimento, escória de alto-forno, cinza volante, água, superplastificante, agregados e idade da mistura, com o objetivo de prever a resistência à compressão do concreto.

Além da modelagem preditiva, o notebook inclui análise exploratória para entender distribuição, correlação entre variáveis e diferenças entre categorias de resistência, o que ajuda a interpretar melhor o comportamento dos dados.

<div align="center">
  <img src="./assets/grafico 2.png" alt="tip" width="800" />
</div>

## Objetivo

O objetivo principal é construir um modelo capaz de prever a resistência à compressão do concreto a partir de variáveis numéricas de composição e idade.

Esse tipo de problema pode apoiar:

- estimativas de desempenho do material;
- análises comparativas entre composições;
- apoio a estudos de engenharia de materiais;
- aplicações de machine learning em contexto industrial.

<div align="center">
  <img src="./assets/grafico 1.png" alt="tip" width="800" />
</div>

## Variáveis utilizadas

A base contém as seguintes variáveis principais:

- `Cement`
- `Blast Furnace Slag`
- `Fly Ash`
- `Water`
- `Superplasticizer`
- `Coarse Aggregate`
- `Fine Aggregate`
- `Age`
- `Concrete compressive strength`

Também foi criada uma variável categórica auxiliar:

- `Strength Category`

## Análise exploratória

O notebook apresenta uma etapa de exploração dos dados com foco em estatística descritiva, correlação e distribuição das variáveis.

Entre os principais pontos observados:

- a base possui 2020 registros e não apresenta valores nulos nas colunas analisadas;
- a variável alvo `Concrete compressive strength` possui média de 35.89 MPa;
- a categoria `Baixa` representa 90.64% dos casos, enquanto `Alto` representa 9.36%;
- as maiores correlações positivas com a resistência aparecem em `Superplasticizer` (0.3298), `Cement` (0.3278) e `Age` (0.2902).

## Modelagem

O projeto foi estruturado como um problema de regressão supervisionada para prever a resistência à compressão.

O notebook inclui:

- preparação da base;
- análise de correlação;
- criação de variável categórica de apoio;
- treinamento e avaliação de modelos;
- interpretação de coeficientes.

Entre os resultados registrados no notebook:

- **MAE:** 5.0085
- **R²:** 0.8177

Em outro cenário/modelo avaliado:

- **MAE:** 9.2613
- **R²:** 0.5265

## Principais insights

Alguns insights relevantes do projeto:

- concretos classificados como resistência **Alta** apresentam média de 68.8 MPa;
- concretos classificados como resistência **Baixa** apresentam média de 32.5 MPa;
- a distribuição das categorias mostra forte predominância da classe de baixa resistência;
- variáveis ligadas à composição da mistura e ao tempo de cura apresentam relação importante com a resistência final.

## Tecnologias e bibliotecas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Estrutura do projeto

```bash
regressao-resistencia-concreto/
├─ RID157020_Desfio_Regressao-4.ipynb
├─ assets/
│  ├─ grafico-1-3.jpg
│  ├─ grafico-2-2.jpg
│  └─ grafico-3.jpg
└─ README.md
```

## Visualizações incluídas

O projeto inclui visualizações para apoiar a interpretação dos dados e do modelo, como:

- matriz de correlação;
- gráficos de distribuição;
- comparações entre categorias de resistência;
- análise visual da dispersão das variáveis.

## Aplicações

Este tipo de projeto pode ser aplicado em cenários como:

- controle de qualidade de materiais;
- engenharia civil e dos materiais;
- previsão de propriedades físicas;
- estudos acadêmicos em regressão e ciência de dados.

## Próximos passos

- comparar diferentes algoritmos de regressão;
- aplicar validação cruzada;
- testar seleção de variáveis;
- avaliar técnicas de balanceamento para a variável categórica auxiliar;
- incluir interpretação mais aprofundada dos erros do modelo.

## Autor

Projeto desenvolvido para fins de estudo e portfólio em ciência de dados, machine learning e análise aplicada à engenharia.
