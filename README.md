# classificador_AVCs

APS 6 - Álgebra Linear e Teoria da Informação - 2021.1

## Integrantes do grupo
* [Isabelle da Silva Santos](https://github.com/isabelleatt)
* [Livia Tanaka](https://github.com/liviatanaka)

* No `README.md` do repositório, deve haver um resumo, com até 400 palavras, explicando qual foi a metodologia usada, quais foram os principais resultados encontrados, e o que o grupo descobriu sobre AVCs à partir da análise dos dados.

## Metodologia - Explicação

####  Classificação Linear

No nosso código, a função de perda utilizada é o erro quadrático médio, que é a média das diferenças entre as saídas preditas e as saídas reais ao quadrado. O modelo é treinado utilizando-se o gradiente descendente, um método de otimização iterativo que atualiza os parâmetros do modelo na direção oposta ao gradiente da função de perda.

####  Árvore de Decisão

Máxima entropia. 

## Resultados 

features relevante de causa para avs (intersecção do linear e da árvore):

* Hipertensão
* Ex fumante 
* Obesidade 
* Idoso

http://www.ojs.unirg.edu.br/index.php/2/article/view/472
https://oswaldocruz.br/revista_academica/content/pdf/Edicao_06_Stephane_sfalsini.pdf

INFLUÊNCIA DO TABAGISMO E DA GLICEMIA NO TRATAMENTO
DO AVC EM PACIENTES INTERNADOS

features relevantes para prevenção de AVC (intersecção do linear e da árvore):

* Residência urbana
* Gênero masculino
* Adultos maduros (Entre 40 e 60 anos)


## Conclusões 

A partir da análise dos dados, foi possível descobrir que o Acidênte Vascular Cerebral (AVC) é uma doença que pode ser causada por diversos fatores, como por exemplo, o tabagismo, o consumo de álcool, a hipertensão, a diabetes, entre outros. Além disso, foi possível observar que a maioria dos pacientes que sofreram AVCs são do sexo masculino, e que a maioria dos pacientes que não sofreram AVCs são do sexo feminino.
