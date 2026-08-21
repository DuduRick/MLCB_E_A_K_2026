--- RESULTADOS DO LAB 01 (AULA 03) ---
Mensagem: 'Preciso urgente da segunda via da fatura'
Intenção Predita: [segunda_via]
Vocabulário Filtrado (sem stopwords): ['2a', '2a via', 'aberto', 'acordo', 'acordo pagar', 'alterar', 'alterar endereço', 'app', 'atrasada', 'atualizo', 'atualizo dados', 'boleto', 'cadastramento', 'dados', 'dados residenciais', 'débito', 'débito aberto', 'dívida', 'emitir', 'emitir segunda', 'endereço', 'endereço cadastramento', 'fatura', 'fatura atrasada', 'fazer', 'fazer um', 'gostaria', 'gostaria alterar', 'negociar', 'negociar pagamento', 'no', 'no app', 'onde', 'onde atualizo', 'pagamento', 'pagamento dívida', 'pagar', 'pagar débito', 'posso', 'posso emitir', 'residenciais', 'residenciais no', 'segunda', 'segunda via', 'um', 'um acordo', 'via', 'via boleto', 'via fatura']

1 - A remoção das stopwords diminui o tamanho do vocabulario, tirando palavras comuns como "de", "a", "como" e "preciso", assim, o modelo foca mais nas palavras importantes.

2 - Faz o modelo analisar palavras sozinhas e tambem combinações de duas palavras, como "segunda via"

3 - As palavras genéricas não ajudam muito a identificar a intenção, removendo elas, o modelo consegue dar mais atenção as palavras importantes da frase

--- RESULTADOS DO LAB 02 (AULA 03) ---

--- Relatório de Classificação ---
                     precision    recall  f1-score   support

horario_atendimento       0.50      1.00      0.67         1
        localizacao       0.00      0.00      0.00         1
    troca_devolucao       0.00      0.00      0.00         1

           accuracy                           0.33         3
          macro avg       0.17      0.33      0.22         3
       weighted avg       0.17      0.33      0.22         3

--- Matriz de Confusão ---
[[1 0 0]
 [1 0 0]
 [0 1 0]]

1- Precision mostra quantas previsões feitas pelo modelo estavam certas / o Recallmostra quantos exemplos de uma classe o modelo conseguiu encontrar / F1-Score junta Precision e Recall em uma unica metrica

2 - A diagonal mostra os casos que o modelo classificou corretamente, quanto mais valores nela melhor o resultado

3 - pode enganar quando as classes são desbalanceadas, pois o modelo pode acertar muito a classe maior e errar as menores, por isso, é importante analisar também Precision, Recall e F1-Score

--- RESULTADOS DO LAB 03 (AULA 03) ---

1 - Acuracia via Pipeline: 0.00%

2 - O Pipeline junta o pré-processamento e o treinamento em um único processo, deixando o código mais organizado e evitando etapas manuais.

3 - Ele garante que o mesmo processo de transformação usado no treino seja aplicado ao teste, evitando diferenças no pré-processamento dos dados.




