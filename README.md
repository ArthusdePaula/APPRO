Case submetido para a avaliação da banca na certificação Data Master Ciência de Dados Santander 2023.
Certificação interna composta por prova técnica, realização de case, apresentação para banca com sabatina. Única pessoa de área não ligada diretamente à dados a passar desde o início do projeto.
Case formado por um conjunto de dados sintéticos contendo uma grande quantidade de variáveis; 
•	A primeira tarefa consistia em maximizar o lucro por cliente considerando o contexto que todo cliente classificado como insatisfeito seria alvo de uma ação com custo unitário de R$ 10,00, onde, se falso positivo não haveria ganho, apenas gasto (pois na realidade seira satisfeito), enquanto o verdadeiro positivo receberia uma receita de R$ 100,00 (lucro de R$ 90,00);
•	A segunda tarefa consistia em dar uma nota de 1 a 5 para cada cliente da base teste;
•	A terceira tarefa era encontrar os três grupos naturais que possuíssem os maiores lucros esperados por cliente.
Utilização de técnicas de Limpeza e Preparação de Dados, Análise Exploratória de Dados, seleção de variáveis excluindo correlações mútuas. Modelagem, Validação cruzada, Normalização, Avaliação de métricas do modelo. Por ser uma base desbalanceada comparei a utilização de oversampling que gerou melhora significativa. Modelo final utilizado XGBoost
A matriz de confusão foi o balizador pela lógica do lucro ser basicamente (tp*90 - fp*10).
Para última questão foi utilizado modelo de clusterização utilizando K-means onde utilizei K = 10 e foi possível perceber que 1 cluster se destacou mesmo entre os 3 com maior lucro.
