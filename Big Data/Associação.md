Pode ser um modelo [[aprendizagem não supervisionada]].


- Análise de market Basket 
	- Vejo todos os produtos que vendo e vejo quais possuem mais correlação
	- Também pode existir regras compostas


- Acaba sendo um processo de força bruta de todos com todos, e depois disso verificar a força da correlação.
- O objetivo do algorítmo é gerar quais são as regras que fazem mais sentido dentre todas as que existem.


#### Métricas: 
- Suporte:  quantidade de vezes que há um certo evento em todas os eventos da base
- Confiança: Dentre todos os eventos que um pressuposto ocrre, qual a percentagem do segundo evento ocorrer.
	- Isso significa que o inverso não é verdadeiro, podendo obter resultados diferentes.