WEB Semântica - Forma de estruturar dados na internet que da semântica aos dados
	- Duas informações ligdas por um predicado
	- DBPedia
	- Word2Vec
	
 
[[Pyhton Notebook - Natural Language]]


É muito comum ter classes (categorias) majoritárias com um desbalanceamento muito grande e algumas com quase nenhum dado presente. Nesses casos, NÃO DEVEMOS excluir essas clases minoritárias, já que caso haja a remoção é efetivamente dizer que as classes não existem. Uma melhor forma é conseguir agrupar essas categorias menores em alguma categoria majoritária (alinhando com a galera da lógica de business). Outra opção é gerar a categoria "outros". Caso não, todas essas classes serão parte do seu percentual de erro, o que pode ser aceitável, a depender do caso. 


O maior trabalho em pre-procesamento de texto é encontrar e remover palavras que não são úteis, como artigos, preposições e até mesmo palavras-chave que são comuns aos grupos (exemplo de lula vs bolsonaro, ambos possui "presidente" e "ladrão").

Cascateamento pode ser uma possibilidade para ponder filtrar os grupos em partes cada vez mais únicas.


A importância de cada palavra em cada texto (uma célula de uma linha [texto] e de uma coluna [palavra]) pode ser a contagem direta dos valores, como pode ser calculáda através de métodos a fim de inflacionar a importância de cada palavra. O risco é evitar que esse peso acabe diminuido a importância de outras palavras chave. Em textos de tamanho pequeno (ex.:tweets), a contagem absoluta pode ser suficiente, já que uma plavra que aparece "3" vezes com certeza é muito importante.
O TF (quantidade de repetições em um texto) & DF (quantidade de vezes que a palavra se repete) também é outra forma de identificar o peso de uma palavra. Essa análise, adepender da relação de TF DF pode indicar que a palavra só é usada em casos únicos (inúteis) ou que se repetem em diversos textos (releantes) e outras que aparecem muito em diversos/ todos textos (provavelmente inútil). É importante lembrar que uma coluna deve ter o mesmo significado em todas as linhas. TF DF é #Confia. ! de Typescript, vai que dá certo.

$$ TF|DF(t,d) = TF(t,d).log(\frac{N}{DF(t)})$$
Sendo 'N' o número de documentos, 't' o termo e 'd' o coumento.

Limpeza de dados - NLP
- Retirar caracteres especiais, como \\n, \\'s (posse), \\r, \\t, '    '
- sinais de pontuação utilizando regex '\[^A-Za-z0-9+\]' (essa filtra acentos e ç)
- Converter para minúsculo
-  [[Stop words]]
- Lematização
- Stemmatização
	- Lancaster é mais agressivo
	- Tem o spacy tbm que o prof ta usando ultimamente


Vetorização:


Feature Selection:
- Seleção do número de K (número de atributos)
	- Aplicar a porcentagem com relação ao total da base já que o número pode variar muito a dependar das bases. (Faz um bissect)
	- Cuidado para evitar que a base de dado não fique com linhas vazias, pois isso significa que qualquer modelo que não tenha nenhum feature irá cair naquele tipo específico. Se mais de um tipo estiver com linhas vazias, o modelo não funciona, já que você está dizendo que os parâmetros iguais geram resultados diferentes.



