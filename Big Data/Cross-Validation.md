1. Visa resolver o problema do Houdout, separando toda a base em treino e teste diversas vezes, gerando K modelos, que no final calculará a média e o desvio padrão de todos os modelos. Cada modelo irá mostrar 
2. Pode gerar [[Data Leakage]], caso utilizemos todo o conjunto para calcular parâmetros, mas este pode ser evitado se o pré-procesamento for realizado em cada iteração. ^dfd1a8
3. Muito utilizado em conjunto com o [[Houdout]], separando um conjunto de validação que nunca será mostrado ao modelo, apesar de trazer o mesmo [[Houdout#^f73193|problema que temos no Houdout]], mas reduz overfiting, deixando ele mais evidente, já que é bem mais difícil ocorrer overfiting em "10" faixas diferentes.
4. O pré-processamento deve ser feito a CADA iteração no cross validation, evitando o ponto [[Cross-Validation#^dfd1a8|2]].
5. A definição da base de teste é sequencial (K serparações aletórias sem intersecção, não deve haver dois conjuntos de testes com o mesmo elemento).
6. No final, teremos a média e o Desvio Padrão de todos os K modelos gerados. **O desvio padrão da um indício de se há dados na base que podem ser tratados separadamente ou que nem deveriam estar ali**.
7. Academia utiliza K =10, se a média e desvião padrão estiverem ok, mantém. Caso K seja pouco, performance pode ser ruim e caso K seja elevado a performance é elevada.
	

8.  Stratfied Cross-validation
	1. Mesma coisa do Crossvalidation, porém (NÃO CONSEGUI OUVIR :( É O QUE O PROFESSOR COSTUMA USAR)