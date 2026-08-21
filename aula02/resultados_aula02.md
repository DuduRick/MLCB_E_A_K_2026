-- RESULTADOS DO LAB 01 ---
Mensagem: 'Quero consultar quanto dinheiro tenho' ==> Intenção Predita: [fazer_pix]
Mensagem: 'Pode me ajudar a fazer um pix?' ==> Intenção Predita: [fazer_pix]
Mensagem: 'Gostaria de cancelar meu cartão de crédito' ==> Intenção Predita: [cancelar_conta]

1 - A Mensagem N°1 Está incorreta, pois deveria ter retornado a intenção "consultar_saldo" e retornou "fazer_pix".
2 - A Maneira mais eficiente de resolver o problema seria treinar mais o modelo.
3 - Ele tem a função de prever a possivel intenção.




--- RESULTADOS DO LAB 02 ---
Mensagem de Teste: 'Gostaria de devolver o produto que comprei'
Intenção Predita: troca_devolucao

--- Distribuição de Probabilidades por Classe ---
Classe [duvida_frete]: 27.99%
Classe [rastrear_pedido]: 24.54%
Classe [troca_devolucao]: 47.46%

1 - Sim, o código está correto 
2 - ampliação do dataset, para melhorar a eficiencia e acertividade
3 - ele atua calculando as probabilidades das palavras se encaixarem em cada intenção

--- RESULTADOS DO LAB 03 ---

Acurácia do Modelo: 33.33%

1 - A acurácia varia e é pouco confiável porque o conjunto de teste tem pouquíssimas frases, fazendo com que um único erro altere drasticamente o resultado final sem refletir o mundo real

2 - Ela analisa a presença de palavras-chave vetorizadas e cria divisões em cascata baseadas em ganho de informação, fazendo perguntas do tipo "tem essa palavra?" até chegar na classe

3 - O modelo decora demais os dados de treino e perde a capacidade de generalizar, errando assim que pega frases novas ou diferentes das que já viu

--- RESULTADOS DO LAB 04 ---

Dataset:
                                             mensagem          intencao
0             Quero comprar uma passagem para Orlando  comprar_passagem
1           Gostaria de reservar um voo para Salvador  comprar_passagem
2      Qual o preço da passagem de avião para Lisboa?  comprar_passagem
3   Preciso comprar bilhete aéreo para o Rio de Ja...  comprar_passagem
4       Como faço para cancelar minha reserva de voo?  cancelar_reserva
5          Quero pedir o cancelamento da minha viagem  cancelar_reserva
6         Gostaria de anular minha compra de passagem  cancelar_reserva
7        Preciso cancelar meu voo marcado para amanhã  cancelar_reserva
8       Quero falar com um atendente humano por favor   falar_atendente
9       Pode me transferir para o suporte ao cliente?   falar_atendente
10     Preciso de ajuda com uma pessoa do atendimento   falar_atendente
11   Gostaria de conversar com um operador da agência   falar_atendente

==================================================
--- MOTOR DE NLU: AGÊNCIA DE VIAGENS ---
==================================================
Acurácia no conjunto de teste: 33.33%

--- PREDIÇÃO DE MENSAGENS INÉDITAS ---
Mensagem: 'Gostaria de saber o valor para voar até Paris'
==> Intenção Predita: [comprar_passagem]

Mensagem: 'Quero cancelar o bilhete que comprei ontem'
==> Intenção Predita: [cancelar_reserva]

Mensagem: 'Me transfira para um suporte humano, por favor'
==> Intenção Predita: [falar_atendente]





