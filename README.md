# Análise de Redes Sociais

<p align="center">
  <img src="images/conection.jpeg" >
</p>

**O que são redes Sociais?**

Você deve se deparar diariamente com o termo “redes sociais”, mas você sabe o verdadeiro significado de tal termo?

Muitos, de maneira automática, associam o termo aos sites de relacionamento, como Facebook, LinkedIn, Twitter, Instagran, etc. No entanto, o conceito de “rede social” é conhecido pelos pesquisadores antes mesmo das chamadas “mídias sociais”. Tome como exemplo as pessoas que você conhece/interage na academia que frequenta, elas fazem parte de sua rede social off-line, mesmo que você tenha algumas pessoas adicionadas em seus perfis de sites de relacionamento, sua rede social on-line será diferente de sua rede social off-line, as “redes sociais” na Internet são representações das redes sociais off-line dos indivíduos e suas conexões.

Redes Sociais são formadas por estruturas que representam as relações existentes entre atores, formando o que podemos chamar de tecido social, e que pode ser representado/estudado matematicamente pela Teoria de Grafos, que veremos mais adiante.

**Redes Sociais na Internet**

Todos nós sabemos que a maioria das pessoas se expressa em uma determinada rede social on-line, seja comentando fotos, publicando vídeos, discutindo determinados assuntos, reagindo a Posts, etc. Tudo isso gera o que chamamos de “rastros digitais”, com esses rastros digitais podemos identificar as relações existentes de pessoa com as demais, em outras palavras, criar uma rede de relacionamentos.

Com os avanços tecnológicos proporcionados pelo conceito de Big Data, podemos olhar para esses “rastros digitais” e consequentemente medir, analisar e interpretar as relações existentes entre os atores sociais, verificar como uma informação transita pela rede, quem são as pessoas mais influentes, etc. Tudo isso faz parte da Análise de Redes Sociais (ARS), que veremos no próximo tópico.

**Análise de Redes Sociais**

Efetuar a ARS nada mais é do que verificar a estrutura existente entre os relacionamentos da rede, deixando de lado o viés individualista, que seria olhar para um indivíduo de modo isolado, e focando o estudo na rede como um todo, entre outras palavras seria verificar a estrutura da rede e compreender de modo teórico e epistemológico o papel que o grupo de indivíduos e suas conexões exercem na estrutura da rede.

Um bom exemplo desta análise é saber como uma determinada informação se propaga pela rede e quem seria o melhor ator social para propagar essa informação. Um dos estudos mais interessantes sobre redes sociais off-line é conhecido como Six Degrees of Separation (Seis Graus de Separação), publicado por Stanley Milgram em 1967, como resultado o autor mostra que em média, qualquer pessoa está a seis pessoas de qualquer outra na rede, de maneira complementar, em 2012, Lars Backstrom descobriu que na rede on-line Facebook esse número cai para quatro pessoas.

A ARS é sustentada por uma forte teoria e as métricas existentes nesta teoria nos dão o poder de análise da rede. Logo mais iremos expor de modo simplificado tais métricas.

**Redes Complexas e Grafos**

Uma rede complexa pode ser definida como uma estrutura não trivial podendo ser representado por um grafo, que é composto por um conjunto de vértices (nós) interligados por meio de arestas. Redes Complexas aparecem cotidianamente na modelagem de problemas como, por exemplo, sistemas de transporte, infraestrutura elétrica, progressão de epidemias, redes de Internet, redes sociais e influência política.

**inserir Imagem**

De maneira simplista podemos definir um Grafo G(V,E), como sendo uma das possíveis representações de uma rede complexa, onde G representa o grafo em si, V é o conjunto de vértices/nós e E é o conjunto de arestas. A figura a seguir apresenta um grafo não direcionado em que os vértices são pessoas e as arestas a relação de amizade entre essas pessoas.

**inserir Figura**

A Teoria dos Grafos originou-se com o trabalho do matemático Leonard Euler, uma das contribuição de Euler foi resolver, em 1736, o enigma das pontes de Königsberg, para mais detalhes consulte o link das referências.

**Principais Elementos**

De modo a esclarecer, mesmo que de maneira redundante, para você que não tem nenhuma familiaridade com os termos aparentes na ARS, segue abaixo um breve resumo:

* Grafo – G(V,E): representação matemática e visual de uma rede de atores (nós/vértices) e suas conexões (laços/arestas);
* Vértices – V: são objetos fundamentais de um grafo, eles estabelecem as conexões da rede, em uma rede social, por exemplo as pessoas poderiam ser representadas pelos vértices;
* Arestas – E: são as conexões existentes entre os vértices do grafo, em uma rede social, por exemplo a troca de mensagens entre pessoas pode gerar uma conexão entre elas, e consequentemente uma aresta. Arestas podem indicar desde uma simples conexão até mesmo se esta conexão tem um peso ou é direcionada;
* Grupo, comunidade ou cluster: conjunto de nós aproximados por uma determinada conexão, em uma rede social podemos ter clusters definidos pelo mesmo modo de pensar ou se expressar na rede.

**Métricas de Nó**

Este tipo de métrica mostra o quão central um nó se encontra em determinada rede. Deste modo, veja algumas dessas métricas:

* Grau do nó (degree): representa o número de conexões que um determinado nó tem, em redes sociais esta medida identifica o ator social com maior número de conexões, em outras palavras, o mais influente;
* Grau de Intermediação (betweenness centrality): esta medida se baseia no número de caminhos mínimos que um determinado nó participa, entre outras palavras, ela mostra quem são os hubs da rede, ou nós com papel de “ponte”, quanto maior esta medida mais relevante o nó se torna no espalhamento de um informação, ou até mesmo no bloqueio dela. Nós com alta centralidade de intermediação ocupam posições estratégicas na rede, por terem a função de gatekeeper, ou aquele que dissemina uma informação;
* Grau de Proximidade (closeness centrality): avalia a distância que um nó está em relação aos demais da rede, em ARS esta medida mostra o quão perto um ator social está dos demais na rede, com ela também é possível verificar quanto “tempo” é necessário para que uma informação seja difundida a partir de uma pessoa até todas as outras da rede;
* Centralidade de Autovetor (eingenvector centrality): diferentemente do grau do nó, que mede o número de conexões diretas do nó, a centralidade de autovetor avalia como são estas conexões, ou seja, ela também avalia as conexões indiretas que existem com este nó, mostrando quais nós são mais relevantes em seus grupos. 

**Métricas de Rede**

Este tipo de métrica tem o papel de avaliar a estrutura de uma determinada rede. Deste modo, veja algumas dessas métricas:

* Equilíbrio Social: a base da teoria  de equilíbrio social é que, se dois nós estiverem conectados positivamente, eles deverão estar conectados de maneira semelhante a outro terceiro: ambos devem ter relações positivas ou ambos devem ter relações negativas, esta ideia mostra que as tríades desequilibradas também são instáveis e tendem a desaparecer, enquanto as tríades equilibradas tendem a ser estáveis;
* Coeficiente de Agrupamento (clustering coefficient): esta medida avalia a presença de clusters (grupos) na rede, ela fornece como os nós de uma rede tendem a se agrupar, algumas teorias sociais consideram tríades como sendo unidades essenciais de análise de redes sociais e o coeficiente de agrupamento é a fração de triângulos possíveis que contêm o nó do ego, se existir. Existem dois tipos de coeficiente de agrupamento: o local e o global, o local avalia a inserção individualizada de cada nó, já o global mostra uma visão geral  de aglomeração da rede;
* Densidade: a densidade de um grafo é dada pela relação entre o número de vértices e arestas existentes, um grafo é dito denso quando possui muitas arestas para um determinado número de vértices;
* Homofilia: também chamada de assortividade, mede a tendência de conexão de nós que possuem alguma característica semelhante;
* Buracos Estruturais: em redes sociais é comum a presença de diferentes grupos, e a tendência é que a informação compartilhada em cada grupo seja homogênea, uma vez que o grupo é formado por partilhar das mesmas características, neste cenário os buracos estruturais representam a “inexistência” de conexão entre dois grupos diferentes. A palavra inexistência está escrita entre aspas pois um nó em específico cobre estas falhas na rede, tal nó é chamado de broker, em outras palavras eles servem como corretores do fluxo da informação, eles ocupam uma posição privilegiada na rede quanto ao capital social e acesso estratégico da informação, são responsáveis por permitir a integração de informações diversas nos grupos que liga.
* Cliques: a partir dos cliques pode-se descobrir as chamadas “panelinhas”, ou subgrupos altamente coesos em uma rede social, estes subgrupos cooperam estreitamente entre si e se mostram intimamente conectados;
* Comunidades: é uma propriedade comum em redes sociais, que representa “ciclos de amigos comuns”, onde todo membro conhece todos os outros membros, é natural que indivíduos que partilham dos mesmos interesses, ou tenham alguma similaridade, formem grupos ou comunidades, em redes complexas também chamados de clusters, onde o alto grau de conexão entre os nós é decisivo para a formação dos grupos;
      
*Bibliografia:* 

1. ARIF, T. The mathematics of social network analysis: metrics for academic
social networks. Int. J. Comput. Appl. Technol. Res. 4 (12), 889–893, 2015

2. BACKSTRON, L. et al. Four degrees of separation. Proceedings of WebSci’12. New York: ACM, 2012

3. BARABÁSI, A. L.; Network Science. :Cambridge University Press, 2016

4. EULER, L. Solutio problematis ad geometriam situs pertinentis. Disponível em
<https://scholarlycommons.pacific.edu/cgi/viewcontent.cgi?article=1052&context=euler-works>. Acesso: 17 jan. 2020

5. GABARDO, A. C.; Análise de Redes Sociais: uma Visão Computacional. São Paulo: Novatec, 2015

6. LAZEGA, E.; HIGGINS, S. S.; Redes Sociais e Estruturas Relacionais. Belo Horizonte: Fino Traço, 2014

7. MILGRAN, S. The Small Word Experiment. Psychology Today, v. 1, n. 1, 1967. Disponível em: <https://snap.stanford.edu/class/cs224w-readings/milgram67smallworld.pdf>. Acesso em:17 jan. 2020 

8. NEWMAN, M. E. J. Networks: An Introduction. New York: Oxford University Press Inc., 2010

9. RECUERO, R.; BASTOS, M.; ZAGO, G. Análise de redes para mídia social. Porto Alegre: Sulina, 2018

10. ZINOVIEV, D. Complex Network Analysis in Python: Recognize - Construct - Visualize - Analyze – Interpret. Pragmatic Bookshelf, 2018
