Respondam às seguintes questões por palavras vossas:
As Três Formas de Inclusão de CSS: Quais são as três formas de aplicar CSS a um documento HTML (inline, interno e externo) e por que razão o CSS externo é considerado a melhor prática da indústria? Resposta:  
inline:aplicado diretamente num elemento HTML especifico atraves do atributo style.
interno:escrito dentro de uma ta <style> na secção <head> do documento HTML.
externo:escrito num ficheiro .css separado e ligado ao HTML atraves de uma tag <link>.

Seletores de Tipo vs Classe vs ID: Expliquem a diferença prática entre um seletor de tipo (p), um seletor de classe (.destaque) e um seletor de identificador (#formulario), dando um exemplo de quando se deve usar cada um. Resposta:

seletor de tipo (p):aplica estilos a todos os elementos HTML desse tipo em toda pagina.

seletor classe(.destaque):aplica estilos a qualquer elemento que tenha esse valor no atributo class. Pode ser reutilizado varias vezes na mesma pagina e combinado com outras classes.

seletor de identificador(#formulario):destina-se a um elemento unico e exclusivo na pagina (o valor do atributo id nao deve ser repetido no mesmo documento).Tem maior especificidade do que classes e seletores de tipo.



Seletores Descendentes: Qual é a diferença entre a regra nav, a { ... } (com vírgula) e a regra nav a { ... } (com espaço)? Resposta: 
nav , a {...}(com virgula):E um seletor de grupo(ou lista de seletores).aplica a mesma regra de estilo de forma independente a todos os elementos <nav> e a todas as ligações <a> em qualquer parte do documento, independentemente de estarem dentro de <nav> ou nao.

nav a {...}(com espaço):E um combinador de descendentes.Aplica o estilo apenas as ligações <a> que se encontram dentro de um elemento <nav> (seja como filhos diretos ou aninhados mais profundamente dentro dele).Ligações <a> fora de um <nav> não são afetadas


Depuração com DevTools: Como é que o separador "Styles" das Ferramentas de Programador (DevTools) ajuda um programador a identificar problemas quando uma regra de estilo não está a funcionar? Resposta: 
O separador styles das ferramentas de programador (devTools) ajuda a identificar por que motivo uma regra de estilo nao esta a produzir efeito ao mostrar exatamente com o navegador interpretou o CSS do elemento selecionado:

regras riscadas: indica que a propriedade foi sobreposta por outra regra com maior especificidade, colocada mais abaixo marcada com !important.

avisos / icones de erro ou triângulos:Ajuda a detetar erros de sintaxe,nomes de propriedades invalidos ou valores nao suportados

ordem e origem das regras: permite ver de onde ven cada estilo (folha externa, estilo inline , estilos predefinidos do navegador) e ativar/ desativar caixas de seleção para testar rapidamente o que esta a bloquear ou a alterar o visual.