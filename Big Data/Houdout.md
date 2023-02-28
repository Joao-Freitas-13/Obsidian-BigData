1. Separar a base em conjunto de treino e conjunto e de teste.
2. Cuidado com [[Data Leakage]].
3. Garante que uma porção dos dados nunca serão mostrados ao modelo para treino.
4. Percentual de separação para treino/teste: depende do tamanho da base. 
5. Problemas: Se a parte separada para teste for as intâncias mais confusas, o modelo se torna ruim. Se forem as mais fáceis de classificar, o modelo se torna bom. Uma forma de verificarmos isso é se as estimativas calculadas entre os conjuntos estão relativamente próximas. Caso não estejam, pode indicar um problema. ^f73193