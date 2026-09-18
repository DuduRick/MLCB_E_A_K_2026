LAB 01: Trocando para Árvore de Decisão, o bot continuou acertando as respostas, mas passou a responder sempre com 100% de confiança, até em frases sem sentido. Isso quebrou a regra de transferir para um atendente quando o bot está em dúvida.

LAB 02: Mudando de "média" para "valor mais forte" no jeito de entender a frase, as respostas simples continuaram certas, mas frases mais confusas ficaram menos estáveis. A média (jeito antigo) pareceu funcionar melhor.

LAB 03: Subindo o corte de confiança de 50% para 65% e mostrando esse número no painel, mais mensagens duvidosas devem cair no fallback. Mas se o modelo ainda for a árvore do Lab 01, isso quase não muda nada na prática, porque ela raramente entrega confiança "no meio".

LAB 04: Adicionei a opção de cancelamento de contrato com suas frases e resposta, e o sistema já reconheceu a categoria nova sem precisar mudar mais nada. O risco que percebi é confundir essa categoria com a de segunda via de boleto, já que as duas falam de "contrato" — com poucos exemplos de treino isso pode dar confusão.
