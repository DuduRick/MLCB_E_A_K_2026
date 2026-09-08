Exercício 1

Testei a função com a frase "Gostaria de saber se vocês estão DEVOLVENDO os valores das mesas compradas!!!" e o resultado foi: gostar saber devolver valor meso comprada.

Deu pra perceber que a lematização funcionou bem, tipo "devolvendo" virou "devolver" e "compradas" virou "comprada". Só achei engraçado que "mesas" virou "meso" — o Spacy errou nessa, provavelmente porque o modelo _sm que a gente usa é o mais leve e às vezes trapalha em casos assim.

Exercício 2

A matriz de vetores ficou com 32 linhas (uma por mensagem) e 50 colunas (dimensões do embedding). Usei o glove-wiki-gigaword-50 no lugar do FastText, do jeito que o próprio enunciado já sugeria pra facilitar. Só que esse modelo é em inglês, então ele meio que "não entende" bem o português — isso vai aparecer lá no exercício 3.

Exercício 3

Testei duas frases:

"Quero saber o valor do frete do sofá" — o modelo achou que era trocas_devolucoes, com 79,92% de confiança
"Gostaria de ver receitas de bolo de cenoura" — foi pro fallback certinho, com 47,73% (abaixo dos 50% do limiar)

O fallback funcionou do jeito esperado pra frase que não tem nada a ver com o SAC. Já a primeira eu esperava que desse vendas_orcamento, mas classificou errado. Acho que isso acontece porque só tenho 8 exemplos de cada classe e o embedding em inglês não pega bem as palavras em português.

Exercício 4

Regressão Logística: 100% de acurácia
KNN (k=3): 50% de acurácia

Reflexão do Exercício 

Acho que a Regressão Logística ganhou porque ela olha pra base toda de uma vez pra decidir a fronteira entre as classes, então erra menos mesmo com poucos dados. Já o KNN só olha pros vizinhos mais próximos, e como eu tenho poucos exemplos (só 32), esses vizinhos às vezes acabam sendo de classe errada — por isso ele errou tanto mais.
