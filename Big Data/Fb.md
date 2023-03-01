
$$ F \beta = (1+\beta ²). \frac{precision.recall}{\beta².precision+recall} $$

B>1 => revocação > precisão
B=1 => revocação = precisão
0<B<1 => revocação < precisão

Média matemática harmônica que gera uma estatística entre 0 e 1 que associa as das variáveis para servir de treshold. O Beta é definido pelo usuário com base no problema em questão e o Fb pode servir de indicativo para problemas associados à precisão e à Revocação, como quando apenas um item é selecionado como verdadeiro ou quando todos os itens são selecionados como verdadeiro, respectivamente. Apesar das métricas iniciais serem altas, o Fb será baixo, indicando um problema na análise.