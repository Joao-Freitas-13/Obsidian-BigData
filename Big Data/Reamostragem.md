- Criação ou remoção de informações da base
- Geralmente utilizado em bases desbalanceadas. Em raros casos, pode ser usado para aumentar o número de instâncias de uma base (geralmente não produz bons resultados)
- Não necessáriamente é necessário de uma base balanceada para gerar aprendizado:
	- ![[Pasted image 20230208201457.png]]

#### [[Problemas que podem ser aplicados a reamostragem]]


#### [[Técnicas de Reamostragem]]


#### Reamostragem antes ou depois de separar o banco de testes? 

- Caso separarmos os dados de teste antes de realizar a sobreamostragem, podemos acabar colocando todos os dados da área de decisão nos testes
- Caso realizarmos a reamostragem antes, podemos acabar tendo apenas dados fictícios nos dados de teste.

- Solução: Realizar a reamostragem antes, mas guardar o índice dos dados reais para garantir que apenas dados reais estejam neles. 