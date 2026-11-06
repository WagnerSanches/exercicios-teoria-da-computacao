# Capítulo 5 — Redutibilidade: Exercícios e Problemas

Sipser, *Introdução à Teoria da Computação*, edição brasileira, p. 222–225.

## Resumo

| | Quantidade | Números |
|---|---|---|
| **Total** | **35** | Exercícios 5.1–5.8 · Problemas 5.9–5.35 |
| Com solução no livro (R) | 8 | 5.5, 5.6, 5.7, 5.8, 5.10, 5.11, 5.28, 5.30 (só o item a) |
| **Sem solução no livro** | **27** | 5.1–5.4, 5.9, 5.12–5.27, 5.29, 5.31–5.35 |

Observação: a solução do 5.30 cobre só o item **a**. Os itens **b** e **c** ficam sem resposta no livro.

Legenda: ✅ = tem solução em "Soluções selecionadas" (marcado com R no livro) · ⬜ = sem solução · ★ = problema mais difícil (marcado com * no livro).

---

## Exercícios

### ⬜ 5.1
Mostre que $EQ_{\text{GLC}}$ é indecidível.

### ⬜ 5.2
Mostre que $EQ_{\text{GLC}}$ é co-Turing-reconhecível.

### ⬜ 5.3
Encontre um emparelhamento na seguinte instância do Problema da Correspondência de Post.

$$
\left\{ \left[\frac{\texttt{ab}}{\texttt{abab}}\right], \left[\frac{\texttt{b}}{\texttt{a}}\right], \left[\frac{\texttt{aba}}{\texttt{b}}\right], \left[\frac{\texttt{aa}}{\texttt{a}}\right] \right\}
$$

### ⬜ 5.4
Se $A \le_{\text{m}} B$ e $B$ é uma linguagem regular, isso implica que $A$ seja uma linguagem regular? Por que ou por que não?

### ✅ 5.5
Mostre que $A_{\text{MT}}$ não é redutível por mapeamento a $V_{\text{MT}}$. Em outras palavras, mostre que nenhuma função computável reduz $A_{\text{MT}}$ a $V_{\text{MT}}$. (Dica: Use uma prova por contradição e fatos que você já conhece sobre $A_{\text{MT}}$ e $V_{\text{MT}}$.)

### ✅ 5.6
Mostre que $\le_{\text{m}}$ é uma relação transitiva.

### ✅ 5.7
Mostre que se $A$ é Turing-reconhecível e $A \le_{\text{m}} \overline{A}$, então $A$ é decidível.

### ✅ 5.8
Na prova do Teorema 5.15 modificamos a máquina de Turing $M$ de modo que ela nunca tente mover sua cabeça além da extremidade esquerda da fita. Suponha que não fizéssemos essa modificação a $M$. Modifique a construção do PCP para lidar com esse caso.

---

## Problemas

### ⬜ 5.9
Seja $T = \{\langle M\rangle \mid M \text{ é uma MT que aceita } w^{\mathcal{R}} \text{ sempre que ela aceita } w\}$. Mostre que $T$ é indecidível.

### ✅ 5.10
Considere o problema de se determinar se uma máquina de Turing de duas fitas em algum momento escreve um símbolo não-branco sobre sua segunda fita quando ela é executada sobre a entrada $w$. Formule esse problema como uma linguagem e mostre que ele é indecidível.

### ✅ 5.11
Considere o problema de se determinar se uma máquina de Turing de duas fitas em algum momento escreve um símbolo não-branco sobre sua segunda fita durante o curso de sua computação sobre qualquer cadeia de entrada. Formule esse problema como uma linguagem e mostre que ele é indecidível.

### ⬜ 5.12
Considere o problema de se determinar se uma máquina de Turing de uma única fita em algum momento escreve um símbolo branco sobre um símbolo não-branco durante o curso de sua computação sobre qualquer cadeia. Formule esse problema como uma linguagem e mostre que ele é indecidível.

### ⬜ 5.13
Um ***estado inútil*** em uma máquina de Turing é um estado no qual a máquina nunca entra sobre qualquer que seja a entrada. Considere o problema de se determinar se uma máquina de Turing possui algum estado inútil. Formule esse problema como uma linguagem e mostre que ele é indecidível.

### ⬜ 5.14
Considere o problema de se determinar se uma máquina de Turing $M$ sobre uma entrada $w$, em algum momento, tenta mover sua cabeça para a esquerda, quando ela está sobre a célula de fita mais à esquerda. Formule esse problema como uma linguagem e mostre que ele é indecidível.

### ⬜ 5.15
Considere o problema de se determinar se uma máquina de Turing $M$ sobre uma entrada $w$ tenta mover sua cabeça para a esquerda, em algum ponto, durante sua computação sobre $w$. Formule esse problema como uma linguagem e mostre que ele *é* decidível.

### ⬜ 5.16
Seja $\Gamma = \{0, 1, \sqcup\}$ o alfabeto de fita para todas as MTs neste problema. Defina a ***função do castor atarefado***³ $CA: \mathcal{N} \to \mathcal{N}$ como segue. Para cada valor de $k$, considere todas as MTs de $k$ estados que param quando iniciadas com uma fita em branco. Seja $CA(k)$ o número máximo de 1s que ficam na fita dentre todas essas máquinas. Mostre que $CA$ não é uma função computável.

³ N.R.T.: em inglês, *busy beaver function*.

### ⬜ 5.17
Mostre que o Problema da Correspondência de Post é decidível sobre o alfabeto unário $\Sigma = \{1\}$.

### ⬜ 5.18
Mostre que o Problema da Correspondência de Post é indecidível sobre o alfabeto binário $\Sigma = \{0,1\}$.

### ⬜ 5.19
No *Problema da Correspondência de Post Bobo*, *PCPB*, em cada par, a cadeia superior tem o mesmo comprimento que a cadeia inferior. Mostre que o *PCPB* é decidível.

### ⬜ 5.20
Prove que existe um subconjunto indecidível de $\{1\}^*$.

### ⬜ 5.21
Seja $AMBIG_{\text{GLC}} = \{\langle G\rangle \mid G \text{ é uma GLC ambígua}\}$. Mostre que $AMBIG_{\text{GLC}}$ é indecidível. (Dica: Use uma redução a partir do *PCP*. Dada uma instância

$$
P = \left\{ \left[\frac{t_1}{b_1}\right], \left[\frac{t_2}{b_2}\right], \ldots, \left[\frac{t_k}{b_k}\right] \right\}
$$

do Problema da Correspondência de Post, construa uma GLC $G$ com as regras

$$
\begin{aligned}
S &\to T \mid B \\
T &\to t_1 T \texttt{a}_1 \mid \cdots \mid t_k T \texttt{a}_k \mid t_1 \texttt{a}_1 \mid \cdots \mid t_k \texttt{a}_k \\
B &\to b_1 B \texttt{a}_1 \mid \cdots \mid b_k B \texttt{a}_k \mid b_1 \texttt{a}_1 \mid \cdots \mid b_k \texttt{a}_k ,
\end{aligned}
$$

onde $\texttt{a}_1, \ldots, \texttt{a}_k$ são novos símbolos terminais. Prove que essa redução funciona.)

### ⬜ 5.22
Mostre que $A$ é Turing-reconhecível sse $A \le_{\text{m}} A_{\text{MT}}$.

### ⬜ 5.23
Mostre que $A$ é decidível sse $A \le_{\text{m}} 0^*1^*$.

### ⬜ 5.24
Seja $J = \{w \mid \text{ou } w = 0x \text{ para alguma } x \in A_{\text{MT}}, \text{ ou } w = 1y \text{ para alguma } y \in \overline{A_{\text{MT}}}\}$. Mostre que nem $J$ nem $\overline{J}$ é Turing-reconhecível.

### ⬜ 5.25
Apresente um exemplo de uma linguagem indecidível $B$ tal que $B \le_{\text{m}} \overline{B}$.

### ⬜ 5.26
Defina um ***autômato finito de duas cabeças*** (2AFD) como um autômato finito determinístico que possui duas cabeças de somente-leitura, bidirecionais, que começam na extremidade esquerda da fita de entrada e podem ser controladas independentemente para mover em qualquer direção. A fita de um 2AFD é finita e é longa apenas o suficiente para conter a entrada mais duas células em branco adicionais, uma na extremidade esquerda e outra na extremidade direita, que servem como delimitadores. Um 2AFD aceita sua entrada entrando em um estado de aceitação especial. Por exemplo, um 2AFD pode reconhecer a linguagem $\{\texttt{a}^n\texttt{b}^n\texttt{c}^n \mid n \ge 0\}$.

- **a.** Seja $A_{\text{2AFD}} = \{\langle M, x\rangle \mid M \text{ é um 2AFD e } M \text{ aceita } x\}$. Mostre que $A_{\text{2AFD}}$ é decidível.
- **b.** Seja $V_{\text{2AFD}} = \{\langle M\rangle \mid M \text{ é um 2AFD e } L(M) = \emptyset\}$. Mostre que $V_{\text{2AFD}}$ não é decidível.

### ⬜ 5.27
Um ***autômato finito bidimensional*** (AFD-2DIM) é definido como a seguir. A entrada é um retângulo $m \times n$, para quaisquer $m, n \ge 2$. Os quadrados ao longo da fronteira do retângulo contêm o símbolo # e os quadrados internos contêm símbolos sobre o alfabeto de entrada $\Sigma$. A função de transição é um mapeamento $Q \times \Sigma \to Q \times \{\text{E}, \text{D}, \text{C}, \text{B}\}$ para indicar o próximo estado e a nova posição da cabeça (esquerda, direita, em cima, embaixo). A máquina aceita quando ela entra em um dos estados de aceitação. E rejeita se ela tenta mover para fora do retângulo de entrada ou se ela nunca pára. Duas dessas máquinas são equivalentes se elas aceitam os mesmos retângulos. Considere o problema de determinar se duas dessas máquinas são equivalentes. Formule esse problema como uma linguagem e mostre que ele é indecidível.

### ✅ ★ 5.28
**Teorema de Rice.** Seja $P$ qualquer propriedade não-trivial da linguagem de uma máquina de Turing. Prove que o problema de determinar se a linguagem de uma dada máquina de Turing tem a propriedade $P$ é indecidível.

Em termos mais formais, seja $P$ uma linguagem constituída de descrições de máquinas de Turing, em que $P$ satisfaz duas condições. Primeiro, $P$ é não-trivial — ela contém alguma descrição, mas não todas as descrições de MTs. Segundo, $P$ é uma propriedade da linguagem da MT — quando $L(M_1) = L(M_2)$, temos que $\langle M_1\rangle \in P$ sse $\langle M_2\rangle \in P$. No caso, $M_1$ e $M_2$ são quaisquer MTs. Prove que $P$ é uma linguagem indecidível.

### ⬜ 5.29
Mostre que ambas as condições no Problema 5.28 são necessárias para provar que $P$ é indecidível.

### ✅ 5.30 *(só o item a)*
Use o teorema de Rice, que aparece no Problema 5.28, para provar a indecidibilidade de cada uma das seguintes linguagens.

- ✅ **a.** $INFINITA_{\text{TM}} = \{\langle M\rangle \mid M \text{ é uma MT e } L(M) \text{ é uma linguagem infinita}\}$.
- ⬜ **b.** $\{\langle M\rangle \mid M \text{ é uma MT e } 1011 \in L(M)\}$.
- ⬜ **c.** $TUDO_{\text{TM}} = \{\langle M\rangle \mid M \text{ é uma MT e } L(M) = \Sigma^*\}$.

### ⬜ 5.31
Seja

$$
f(x) = \begin{cases} 3x + 1 & \text{para } x \text{ ímpar} \\ x/2 & \text{para } x \text{ par} \end{cases}
$$

para qualquer número natural $x$. Se começar com um inteiro $x$ e iterar $f$, você produz uma seqüência $x, f(x), f(f(x)), \ldots$ que termina se produzir 1. Por exemplo, se $x = 17$, você obtém a seqüência 17, 52, 26, 13, 40, 20, 10, 5, 16, 8, 4, 2, 1. Extensivos testes por computador mostraram que todo ponto de partida entre 1 e um grande inteiro positivo dá uma seqüência que termina em 1. No entanto, a questão de se todos os pontos de partida positivos propiciam o término em 1 não foi solucionada; ela é denominada o problema $3x + 1$.

Suponha que $A_{\text{MT}}$ fosse decidível por uma MT $H$. Use $H$ para descrever uma MT que seja garantida apresentar a resposta para o problema $3x + 1$.

### ⬜ 5.32
Prove que as duas linguagens seguintes são indecidíveis.

- **a.** $SOBREP_{\text{GLC}} = \{\langle G, H\rangle \mid G \text{ e } H \text{ são GLCs tais que } L(G) \cap L(H) \ne \emptyset\}$. (Dica: Adapte a dica do Problema 5.21.)
- **b.** $LIVRE\text{-}PREF_{\text{GLC}} = \{G \mid G \text{ é uma GLC onde } L(G) \text{ é livre-de-prefixo}\}$.

### ⬜ 5.33
Seja $S = \{\langle M\rangle \mid M \text{ é uma MT e } L(M) = \{\langle M\rangle\}\}$. Mostre que nem $S$, nem $\overline{S}$ é Turing-reconhecível.

### ⬜ 5.34
Considere o problema de determinar se um AP aceita alguma cadeia da forma $\{ww \mid w \in \{0,1\}^*\}$. Use o método da história de computação para mostrar que esse problema é indecidível.

### ⬜ 5.35
Seja $X = \{\langle M, w\rangle \mid M \text{ é uma MT de uma única fita que nunca modifica a porção da fita que contém a entrada } w\}$. $X$ é decidível? Prove sua resposta.
