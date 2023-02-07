

- O algoritmo de agrupamento é um algoritmo que pode ajudar a organizar a base para determinado algorítmo de [[classificação]].
- Exemplo: Carregamento de livros chegou numa biblioteca, vou separar os grupos semelhantes e juntá-los em locais específicos. Caso chegue um novo carregamento, precisarei reoganizar a distribuição dos livros.
- Um método de agrupamento pode ser a distância euclidiana de pontos
	- Esse método é problemático quando há uma quantidade muitogrande de dados, por haver uma grande variação em dados semelhantes
- Outro método é utilizar cosseno
- Para texto: Verifica qual palavra é mais frequente em cada grupo

- As vezes já existe um especialista para rotular a base, tornando desnecessário agrupar a base previamente. 
- As vezes esse método é feito para simplemente poder organizar a base.


- É importante dizer que um algorítimo pode identificar grupos que não são relevantes, como por exemplo agrupar quem é funcionário de um colégio ou não, dentro de uma base de pessoas. Por isso é importante limitar quais são os tipos de dados que temos que fornecer ao algorítimo.


## Agrupamento Hard x Soft

- Uma pessoa pode ser alta e baixa ao mesmo tempo, caso estes sejam os dois critérios. Pode ser baixa em um país e a mesma pessoa ser alta em outro. 
- Um texto é um grande exemplo disso, que pode falar sobre política e saúde, por exemplo, no mesmo texto
- Possível também uma classificação multiclasse.


