# classificador_AVCs

APS 6 - Álgebra Linear e Teoria da Informação - 2023.1

## Integrantes do grupo
* [Isabelle da Silva Santos](https://github.com/isabelleatt)
* [Livia Tanaka](https://github.com/liviatanaka)


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


## Conclusões 

A partir da análise dos dados, foi possível descobrir que o Acidênte Vascular Cerebral (AVC) é uma doença que pode ser causada por diversos fatores, por exemplo, o sobrepeso, a hipertensão, e a idade avançada. Além disso, foi possível observar que o hábito de fumar pode ser uma das causas do AVC, já que o fato de ser fumante apareceu como uma característica relevante de causa. E, em contraste, o fato de nunca ter fumando apareceu como uma característica de prevenção ao AVC. Outras exemplos de características de prevenção que apareceram foram: nível de glicose normal, e morar em um ambiente rural.
