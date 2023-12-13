# Situação problema

A presente análise tem como objetivo auxiliar uma loja na elaboração de possíveis campanhas de marketings e na venda de serviços ou produtos novos.

Para tal é necessário à identificação de grupos de clientes-alvo e quais seriam suas características principais.

Portanto será analisado um dataset contendo algumas informações básicas dos consumidores do shopping onde essa loja está alocada, como a idade, renda, sexo, etc. A partir destas variáveis será elaborado um algoritmo de clusterização em Python para identificar quais seriam os grupos mais importantes para serem focados/trabalhados pela equipe de marketing.

# Análise Exploratória dos Dados

Examinando o glossário do dataset tem-se:
<img src="/customer_clustering/img_project/desc_variaveis.jpg">

Observando a imagem nota-se a presença de três variáveis numéricas e cinco variáveis categóricas.

<img src="/customer_clustering/img_project/null_val.jpg ">

Examinando o dataset carregado com as funções “.info()” e “.duplicated()” não é possível notar a repetição de algum tipo de consumidor em específico ou a presença de dados ausentes. 

Nota-se também que não é possível identificar a qual tipo de ramo a loja analisada pertence por meio das features apresentadas.
Para um entendimento inicial dos dados será realizado uma visualização da distribuição de cada variável isoladamente.

## Variáveis numéricas

### Age
<img src="/customer_clustering/img_project/img_2.jpg ">

Pelos gráficos e pelas tabelas têm-se:

  - A média de idade dos compradores é de aproximadamente 36 anos.
   - Existe uma grande concentração de pessoas com idades entre aproximadamente 25 a 28 anos.
   - A menor idade é de 18 anos e a maior é 76 anos.
   - 75% dos dados está concentrado na faixa abaixo dos 42 anos

### Income

<img src="/customer_clustering/img_project/img_3.jpg ">

Analisando o gráfico e a tabela têm-se:

  -  A média de renda anual é de aproximadamente 121,000 tendo um desvio de 40,000.
  -  É possível identificar visualmente outliers pelo gráfico, apartir da zona dos 200,000 de renda anual.
  -  O mínimo de renda anual é de aproximadamente 35,800 e a máxima é de 309,000.
  -  A maior concentração de valores de renda anual é na faixa de 106,000 à 113,000.

## Variáveis categóricas

Para uma melhor entendimento e vizualização dos dados as features categóricas serão decodificadas com base no 'describe segmentation' disponibilizado.

### Settlement size
<img src="/customer_clustering/img_project/img_4.jpg ">

Analisando o gráfico nota-se:

  -  A maior parte dos dados é composta por pessoas que moram em cidades "small city".
  -  O dataset possui menos menos pessoas vindas de 'big city'.
  -  'mid-size city' e 'big city' possuem aproximadamente a mesma quantidade de dados.


### Education


<img src="/customer_clustering/img_project/img_5.jpg ">

Observando os gráficos nota-se que:

  -  Cerca de 50% do dataset é composto por 'high school' e por 'employee'.
  -  Menos de 2% das pessoas do dataset são 'graduate school'.
  -  Cerca de 30% à 32% do dataset é composto por 'unemployed Occupation'.


### Sex 

<img src="/customer_clustering/img_project/img_6.jpg ">

Analisando os gráficos têm-se:
- A quantidade de pessoas solteiras e não solteiras é praticamente igual neste dataset.
- A quantidade de pessoas do sexo 'male' e 'female' é relativamente igual, tendo uma diferença de cerca de 5% entre eles.
