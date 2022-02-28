# Mais uma introdução às equações diferenciais

``Do you know,'' the Devil confided, ``not even the best mathematicians on other planets - all far ahead of yours - have solved it? Why, there’s a chap on Saturn - he looks something like a mushroom on stilts - who solves partial differential equations mentally; and even he’s given up.'' -- Arthur Porges, ``The Devil and Simon Flagg''


## Mais um texto de equações diferenciais


Bem-vindo a esta proposta de curso introdutório de equações diferenciais! A ideia é que este curso venha logo após os dois primeiros cursos de cálculo (integrais e derivadas de funções de uma e várias variáveis), um curso de geometria analítica e vetores, e talvez um curso introdutório de álgebra linear.

A versão inicial dessas notas está totalmente baseada em slides que usei quando ministrei esse curso em 2020, de forma remota. %O curso foi lecionado remotamente, então os slides eram bem detalhados. %Elas foram melhoradas (será?) para lecionar o curso novamente em 2022.


O objetivo não é que isso seja um livro de EDO - existem excelentes livros de equações diferenciais, em especial as referências 1, 2, 3, 4 e 5 que recomendo que você leia e procure exercícios para fazer. Essas notas são só para organizar meu curso.

## O que esse material cobre?

Estas notas cobrem a ementa atual do curso de Cálculo III ministrado pelo IMECC/Unicamp, complementado por alguns conteúdos que são importantes para alunos do Cursão e algumas engenharias. %O material está estruturado para que cada capítulo seja, \textit{mais ou menos}, uma ou duas aulas.

Essa apostila cobre:


1. Equações diferenciais ordinárias de primeira ordem. Equações lineares. Teorema de existência e unicidade. Equações separáveis, exatas, fatores integrantes. Outros métodos substitutivos. Equações homogêneas.
2. Equações diferenciais ordinárias lineares de ordem superior. Princípio da su\-per\-po\-sição. Wronskiano. Equações homogêneas com coeficientes constantes. Métodos: Coeficientes indeterminados, variação dos parâmetros. Redução de ordem. Equações de Euler.
3. Transformadas de Laplace. Solução de problemas de valor inicial. Funções degrau. Funções impulso. A integral de convolução.
4. Seqüências. Séries numéricas. Testes da integral, da comparação, do limite, da razão, da raiz, etc. Séries de potências. Séries de Taylor.
5. Sistemas lineares. Exponencial matricial. Método da transformada de Laplace. Método da eliminação. Método de autovalores. Método dos coeficientes indeterminados. Método de variação dos parâmetros. 
6. Soluções de equações diferenciais ordinárias por séries de potências e por séries de Frobenius.
7. Funções periódicas. Séries de Fourier. Equações diferenciais parciais. Problemas de fronteira. Equações da onda e do calor. Método de separação de variáveis. Equação de Laplace. Problema de Dirichlet.



## Abordagem computacional

Nestas notas você encontra alguma coisa sobre soluções computacionais de equações diferenciais, sejam algébricas ou numéricas.

A maior parte dos gráficos aqui dessa apostila foi feita no Python (outros no Mathematica). No site

http://www.ime.unicamp.br/~rmiranda/code/python.html

você encontra um tutorial de Python, com alguns comandos básicos. Alguns dos exercícios também exigem que você use alguma ferramenta computacional, e nesse ponto o tutorial acima também pode ajudar.


## Bibliografia complementar

Estas notas de aula foram baseadas em várias referências bibliográficas. Você encontra algumas citações pelo livro, mas as referências básicas foram:


1. William F. Trench, Elementary Differential Equations (2013). Faculty Authored and Edited Books \& CDs. 8. \url{https://digitalcommons.trinity.edu/mono/8/}
2. Djairo Guedes de Figueiredo, Equações diferenciais aplicadas, 12o Coloquio Brasileiro de Matematica, Rio de Janeiro, RJ : IMPA, 1979. (515.35 F469e)
3. George F. Simmons, Differential equations with applications and historical notes, Boca Raton, FL: CRC/Taylor \& Francis, c2017. (515.35 Si47d) (gosta de notas históricas? este é seu livro! - aliás, qualquer livro do Simmons é muito bom)
4. D. G. Zill, Equações Diferenciais com Aplicações em Modelagem, Cengage Learning, 2011. (aqui tem algumas aplicações bem legais)
5. Gilbert Strang, Differential equations and linear algebra, Wellesley, MA: Wellesley-Cambridge Press, 2014. (515.35 St81d) (mais um clássico do Strang, pra quem gosta dos livros dele como eu - ele é o autor das vídeo-aulas do MIT, que são muito boas!)
6. William E. Boyce, Richard C. DiPrima, Elementary differential equations and boundary value problems, Hoboken, NJ: John Wiley \& Sons, c2005. (515.35 B692e) (esse livro é uma referência básica do assunto, mas eu não gosto da estrutura do livro)
7. Djairo Guedes Figueiredo \& Aloisio Freiria Neves, Equações diferenciais aplicadas, Rio de Janeiro, RJ: IMPA, 2008. (515.35 F469e)
8. Elon Lages Lima, Curso de Análise, vol. 1, SBM/IMPA. (para a parte de sequências e séries)
9. Djairo Guedes de Figueiredo, Análise I, LTC. (para a parte de sequências e séries)
10. M. Fogiel, David R. Arterburn \& outros, The differential equations problem solver: a complete solution guide to any textbook, Piscataway, NJ: REA, c1998. (código da biblioteca 515.35 D568) (todos os exercícios do mundo resolvidos - só temos um na biblioteca!)
11. Morris W. Hirsch and Stephen Smale, Differential equations, dynamical systems and linear algebra, New York, NY: Academic Press, c1974 (515.35 H615d) (para quem quer estudar um pouco mais de sistemas dinâmicos)
12. Morris W. Hirsch, Stephen Smale \& Robert L. Devaney, Differential equations, dynamical systems, and an introduction to chaos, Amsterdam, Elsevier Academic Press, c2004. (515.35 H615d) (é uma reedição da ref anterior, agora com figuras melhores)
13. Math22 at Harvard: https://people.math.harvard.edu/~knill/teaching/math22b2019/ (visitem!)
14. Paul’s Online Notes: http://tutorial.math.lamar.edu/Classes/DE/DE.aspx (ótimas notas, com ótimos exemplos)
15. Math24 - Differential Equations: https://math24.net/topics-differential-equations.html (material excelente! veja os exemplos resolvidos de lá.)
16. Coleção Schaum de Equações Diferenciais (código da biblioteca 515.35 B789d ou 515.35076 Ay74e) (o REA é melhor, mas aqui também tem muitos exercícios resolvidos)

## Sobre o ensino de equações diferenciais}

Existe um texto bem legal do matemático ítalo-americano Gian-Carlo Rota que eu gosto muito: \textit{Ten lessons I wish I had learned before I started teaching differential equations} (\url{http://www.ime.unicamp.br/~rmiranda/cursos/2020-1-ma311-b/pdfs/rota-ode.pdf}). Recomendo você clicar no link e ler o texto, mas vou fazer um breve resumo dele aqui.

No texto, aparentemente escrito em 2015, prof. Rota dá 10 ``conselhos'' para um bom curso introdutório de equações diferenciais. Eles são:

\begin{enumerate}
\item A maioria do material ensinado atualmente é obsoleto.
\item Ensine o mínimo sobre equações de primeira ordem.
\item Equações diferenciais lineares com coeficientes constantes são muito importantes.
\item Ensine mudança de variáveis.
\item Ignore teoremas de existência e unicidade.
\item Sistemas lineares com coeficientes constantes são o filé com batatas do curso.
\item Fique longe de formas diferenciais.
\item Evite problemas que envolvem modelagem.
\item Dê uma motivação clara para a Transformada de Laplace.
\item Ensine conceitos ao invés de truques.
\end{enumerate}

\bigskip

Cada item é devidamente justificado no texto do prof. Rota. Com exceção do item 5 e talvez do item 7, eu concordo com todos os outros.

Sobre o ensino de teoremas de existência e unicidade, acho que eles são importantes mesmo num curso introdutório. A ideia de que estamos procurando solução para uma equação que não sabemos se tem solução me parece estranha. Por outro lado, é bom ter em mente que em termos de equações diferenciais, ``existir solução'' é diferente de ``vou exibir uma solução explícita'', mais ou menos como já acontece no Teorema Fundamental do Cálculo: a função $$F(x)=\int_0^x e^{t^2},dt.$$ primitiva de $f(t)=e^{t^2}$, existe, só não sabemos exibí-la em termos de funções elementares (aliás, leia sobre isso aqui).

Em todo caso, pode ser uma boa ideia introduzir o Teorema de Picard, e falar um pouco sobre convergência de sequências de funções, ainda que o assunto fique pouco formal. Num primeiro momento, optei por enunciar sem demonstração os resultados. No futuro, tudo estará demonstrado num apêndice.

Sobre as formas diferenciais.. bem, depende. Elas ajudam a ``justificar'' o motivo de aparentemente operarmos com $dy/dx$ como se isso fosse uma fração. É o assunto que dá suporte à notação de Leibniz. É preciso ter boa base de álgebra linear para poder acompanhar. No texto, vamos usar isso de modo intuitivo.%, e num apêndice eu colocarei a teoria necessária pra entender.

Outro assunto é a introdução de coisas ``computacionais''. Mesmo se você for aquele matemático puro que inverte matrizes $11\times 11$ na mão, é importante ter um pouco de conhecimento sobre ferramentas computacionais para matemática - pois as matrizes podem ser $111\times 111$ (bom, em teoria é só pegar mais papel, mas..).

O computador, por enquanto, não substitui o conhecimento - ele faz o que a gente manda. Mas não faz tudo, e principalmente se você estiver trabalhando em coisas qualitativas que exigem precisão, não vai adiantar muito pegar a solução numérica. Mas é bom saber fazer simulações e métodos computacionais, no mínimo, ajudam a ganhar intuição sobre os problemas.% Eu vou fornecer quase todos os códigos que vocês precisarem, mas talvez eles tenham que ser adaptados. Eu sou programar? Não, mas o Google sabe. Como faremos coisas simples, provavelmente alguém já teve sua dúvida e você vai achar uma dica aí pela internet.
%
%
\section*{Copyright}

Estas notas de aula estão regidas pela Licença Pública Creative Commons Atribuição 4.0 Internacional: \url{https://creativecommons.org/licenses/by/4.0/legalcode.pt} (veja um resumo clicando aqui: \url{https://creativecommons.org/licenses/by/4.0/deed.pt_BR}.
