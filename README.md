# classificador_AVCs

APS 6 - Álgebra Linear e Teoria da Informação - 2023.1

## Integrantes do grupo
* [Isabelle da Silva Santos](https://github.com/isabelleatt)
* [Livia Tanaka](https://github.com/liviatanaka)

## Introdução

O "Classificador AVCs" é uma APS (Atividade Prática Supervisionada) desenvolvido para a disciplina de Álgebra Linear e Teoria da Informação, ministrada pelo professor Tiago Fernandes Tavares.
Este projeto tem como objetivo a criação e avaliação de dois tipos de classificadores, linear e por árvore de decisão, para a predição de AVCs com base em uma base de dados disponível no [Kaggle](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset). Será utilizada a medida de acurácia para avaliar o desempenho dos classificadores, considerando uma hipótese nula de que a acurácia deve ser comparada com um classificador que sempre "chuta" a classe mais frequente no conjunto de dados. Além disso, serão analisados os fatores de risco para AVCs identificados pelos classificadores e verificado se esses fatores já foram identificados em estudos publicados anteriormente. 

## Metodologia - Explicação

####  Classificação Linear

No nosso código, a função de perda utilizada é o erro quadrático médio, que é a média das diferenças entre as saídas preditas e as saídas reais ao quadrado. O modelo é treinado utilizando-se o gradiente descendente, um método de otimização iterativo que atualiza os parâmetros do modelo na direção oposta ao gradiente da função de perda.

####  Árvore de Decisão

A árvore de decisão é construída levando em consideração a entropia de cada característica para determinar se o paciente teve ou não um AVC. Desse modo, a árvore pontua cada uma das características com valor proporcional a relevância da característica tanto como causa, quanto como prevenção.

## Resultados 

features relevante de causa para avs (intersecção do linear e da árvore):

* Hipertensão
* Fumante 
* Sobrepeso
* Idoso

http://www.ojs.unirg.edu.br/index.php/2/article/view/472
https://oswaldocruz.br/revista_academica/content/pdf/Edicao_06_Stephane_sfalsini.pdf

INFLUÊNCIA DO TABAGISMO E DA GLICEMIA NO TRATAMENTO
DO AVC EM PACIENTES INTERNADOS

features relevantes para prevenção de AVC (intersecção do linear e da árvore):

* Nunca fumou
* Nível de glicose normal
* Tipo de residência: Rural

### Tabagismo como fator de risco para AVC

Os resultados dos classificadores apresentados indicam que o tabagismo é um importante fator de risco para AVC. Tanto o classificador linear quanto o por árvore de decisão identificaram a variável `smoking_status_smokes` como uma das mais importantes para a predição de AVCs, com pesos de 83 e 183, respectivamente. Além disso, o segundo classificador também identificou a variável `smoking_status_formerly` smoked" como relevante, com peso de 159.

Esses resultados estão em consonância com estudos confiáveis realizados por órgãos de saúde renomados, como a Organização Mundial da Saúde (OMS). De acordo com a OMS, o tabagismo é um dos [principais fatores de risco para doenças cardiovasculares, incluindo o AVC](https://www.who.int/health-topics/cardiovascular-diseases#tab=tab_1). A exposição à fumaça do cigarro, seja por meio do próprio tabagismo ou de outras pessoas que fumam, aumenta o risco de formação de placas de gordura nas artérias, além de aumentar a pressão arterial e provocar inflamações no organismo. 

O artigo "Abordagem do tabagismo: estratégia para redução de fator de risco modificável para AVC" escrito pela professora Renata Cruz Soares de Azevedo associada do Departamento de Psiquiatria (DP) da Faculdade de Ciências Médicas (FCM) da Universidade Estadual de Campinas (UNICAMP), também aponta o tabagismo como um fator de risco para AVC. Segundo o artigo, "Das 25 doenças relacionadas ao hábito de fumar, todas são causa de morte, sendo as principais: doenças cardiovasculares (43%), câncer (36%) e doenças respiratórias (20%)." Além disso, o Ministério da Saúde brasileiro também reconhece a [importância do tabagismo como fator de risco para doenças cardiovasculares](https://www.gov.br/saude/pt-br/assuntos/saude-de-a-a-z/a/avc), incluindo o AVC. 


## Conclusões 

A partir da análise dos dados, foi possível descobrir que o Acidênte Vascular Cerebral (AVC) é uma doença que pode ser causada por diversos fatores, por exemplo, o sobrepeso, a hipertensão, e a idade avançada. Além disso, foi possível observar que o hábito de fumar pode ser uma das causas do AVC, já que o fato de ser fumante apareceu como uma característica relevante de causa. E, em contraste, o fato de nunca ter fumando apareceu como uma característica de prevenção ao AVC. Outras exemplos de características de prevenção que apareceram foram: nível de glicose normal, e morar em um ambiente rural.
