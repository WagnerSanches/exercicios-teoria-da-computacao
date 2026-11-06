# Capítulo 5 — Redutibilidade: Exercícios e Problemas (1ª edição)

Sipser, *Uma Introdução à Teoria da Computação*, tradução da 1ª edição (PDF), p. 170–172.

## Resumo

| | Quantidade | Números (1ª ed.) |
|---|---|---|
| **Total** | **23** | Exercícios 5.1–5.8 · Problemas 5.9–5.23 |
| Com resposta na 2ª ed. | 6 | 5.5, 5.6, 5.7, 5.8, 5.16, 5.22 |
| **Sem resposta** | **17** | 5.1–5.4, 5.9–5.15, 5.17–5.21, 5.23 |

As respostas ficam em "Soluções selecionadas" do capítulo 5 da **2ª edição** (p. 225–227), com o número da 2ª edição indicado em cada exercício.

Legenda: ✅ = tem resposta na 2ª ed. · ⬜ = sem resposta · ★ = problema mais difícil (marcado com * no livro).

### Correspondência 1ª → 2ª edição

| 1ª ed. | 2ª ed. | Resposta? |
|---|---|---|
| 5.1 | 5.1 | ⬜ |
| 5.2 | 5.2 | ⬜ |
| 5.3 | 5.3 | ⬜ |
| 5.4 | 5.4 | ⬜ |
| 5.5 | 5.5 | ✅ |
| 5.6 | 5.6 | ✅ |
| 5.7 | 5.7 | ✅ |
| 5.8 | 5.8 | ✅ |
| 5.9 | 5.22 (uma das direções) | ⬜ |
| 5.10 | 5.24 | ⬜ |
| 5.11 | 5.25 | ⬜ |
| 5.12 | 5.9 | ⬜ |
| 5.13 | 5.13 | ⬜ |
| 5.14 | 5.14 | ⬜ |
| 5.15 | 5.15 | ⬜ |
| 5.16 | 5.10 e 5.11 | ✅ |
| 5.17 | 5.17 | ⬜ |
| 5.18 | 5.18 | ⬜ |
| 5.19 | 5.21 | ⬜ |
| 5.20 | 5.26 | ⬜ |
| 5.21 | 5.27 | ⬜ |
| 5.22 | 5.28 | ✅ |
| 5.23 | 5.29 | ⬜ |

---

## Exercícios

### ⬜ 5.1
*2ª ed.: 5.1*

Mostre que $EQ_{\text{GLC}}$ é indecidível.

### ⬜ 5.2
*2ª ed.: 5.2*

Mostre que $EQ_{\text{GLC}}$ é co-Turing-reconhecível.

### ⬜ 5.3
*2ª ed.: 5.3*

Encontre um emparelhamento na seguinte instância do PCP.

$$
\left\{ \left[\frac{\texttt{ab}}{\texttt{abab}}\right], \left[\frac{\texttt{b}}{\texttt{a}}\right], \left[\frac{\texttt{aba}}{\texttt{b}}\right], \left[\frac{\texttt{aa}}{\texttt{a}}\right] \right\}
$$

### ⬜ 5.4
*2ª ed.: 5.4*

Se $A \le_{\text{m}} B$ e $B$ é uma linguagem regular, isso implica que $A$ seja uma linguagem regular? Por que ou por que não?

### ✅ 5.5
*2ª ed.: 5.5 — resposta na p. 225*

Mostre que $A_{\text{MT}}$ não é redutível por mapeamento a $V_{\text{MT}}$.

### ✅ 5.6
*2ª ed.: 5.6 — resposta na p. 225*

Mostre que $\le_{\text{m}}$ é uma relação transitiva.

### ✅ 5.7
*2ª ed.: 5.7 — resposta na p. 226*

Mostre que se $A$ é Turing-reconhecível e $A \le_{\text{m}} \overline{A}$, então $A$ é decidível.

### ✅ 5.8
*2ª ed.: 5.8 — resposta na p. 226 (lá o teorema citado é o 5.15, que é o 5.11 desta edição)*

Na prova do Teorema 5.11 modficamos a máquina de Turing $M$ de modo que ela nunca tenta mover sua cabeça para fora da extremidade esquerda da fita. Suponha que não fizéssemos essa modificação em $M$. Como teríamos que modificar a construção do PCP para lidar com esse caso?

---

## Problemas

### ⬜ 5.9
*2ª ed.: 5.22 (lá pede as duas direções: "A é Turing-reconhecível sse A ≤m A_MT")*

Mostre que todos os problemas Turing-reconhecíveis reduzem por mapeamento a $A_{\text{MT}}$.

### ⬜ 5.10
*2ª ed.: 5.24*

Seja $J = \{w \mid w = \texttt{0}x \text{ para algum } x \in A_{\text{MT}} \text{ ou } w = \texttt{1}y \text{ para algum } y \in \overline{A_{\text{MT}}}\}$. Mostre que nem $J$ nem $\overline{J}$ é Turing-reconhecível.

### ⬜ 5.11
*2ª ed.: 5.25*

Dê um exemplo de uma linguagem indecidível $B$, onde $B \le_{\text{m}} \overline{B}$.

### ⬜ 5.12
*2ª ed.: 5.9*

Seja $S = \{\langle M\rangle \mid M \text{ é uma MT que aceita } w^{\mathcal{R}} \text{ sempre que ela aceita } w\}$. Mostre que $S$ é indecidível.

### ⬜ 5.13
*2ª ed.: 5.13*

Um ***estado inútil*** em uma máquina de Turing é aquele no qual a máquina nunca entra sobre nenhuma entrada. Considere o problema de se testar se uma máquina de Turing tem quaisquer estados inúteis. Formule esse problema como uma linguagem e mostre que ele é indecidível.

### ⬜ 5.14
*2ª ed.: 5.14*

Considere o problema de se testar se uma máquina de Turing sobre uma entrada $w$ em algum momento move sua cabeça para a esquerda quando sua cabeça está sobre a célula mais à esquerda. Formule esse problema como uma linguagem e mostre que ele é indecidível.

### ⬜ 5.15
*2ª ed.: 5.15*

Considere o problema de se testar se uma máquina de Turing sobre uma entrada $w$ em algum momento move sua cabeça para a esquerda em algum ponto durante sua computação sobre $w$. Formule esse problema como uma linguagem e mostre que ele *é* decidível.

### ✅ 5.16
*2ª ed.: 5.10 e 5.11 — respostas na p. 226. A 2ª ed. divide este problema em dois: 5.10 (sobre uma entrada $w$ dada) e 5.11 (sobre alguma entrada). As duas versões têm resposta.*

Considere o problema de se testar se uma máquina de Turing de duas-fitas em algum momento escreve um símbolo não-branco na sua segunda fita. Formule esse problema como uma linguagem e mostre que ele é indecidível.

### ⬜ 5.17
*2ª ed.: 5.17*

Mostre que o PCP é decidível sobre um alfabeto unário, ou seja, sobre o alfabeto $\Sigma = \{\texttt{1}\}$.

### ⬜ 5.18
*2ª ed.: 5.18*

Mostre que o PCP é indecidível sobre um alfabeto binário, ou seja, sobre o alfabeto $\Sigma = \{\texttt{0}, \texttt{1}\}$.

### ⬜ 5.19
*2ª ed.: 5.21*

Seja $AMBIG_{\text{GLC}} = \{\langle G\rangle \mid G \text{ é uma GLC ambígua}\}$. Mostre que $AMBIG_{\text{GLC}}$ é indecidível. (Dica: Use uma redução do PCP. Dê uma instância

$$
P = \left\{ \left[\frac{t_1}{b_1}\right], \left[\frac{t_2}{b_2}\right], \ldots, \left[\frac{t_k}{b_k}\right] \right\},
$$

do PCP, construa uma GLC $G$ com as regras

$$
\begin{aligned}
S &\to T \mid B \\
T &\to t_1 T \texttt{a}_1 \mid \cdots \mid t_k T \texttt{a}_k \mid t_1 \texttt{a}_1 \mid \cdots \mid t_k \texttt{a}_k \\
B &\to b_1 B \texttt{a}_1 \mid \cdots \mid b_k B \texttt{a}_k \mid b_1 \texttt{a}_1 \mid \cdots \mid b_k \texttt{a}_k ,
\end{aligned}
$$

onde $\texttt{a}_1, \ldots, \texttt{a}_k$ são novos símbolos terminais. Prove que essa redução funciona.)

### ⬜ 5.20
*2ª ed.: 5.26*

Defina um ***autômato finito de duas-cabeças*** (2AFD) como sendo um autômato finito determinístico que duas cabeças de somente-leitura, bidirecionais, que começam na extremidade esquerda da fita de entrada e podem ser controladas independentemente para mover em qualquer direção. A fita de um 2AFD é finita e é justamente longa o suficiente para conter a entrada mais duas células de fita em branco, uma na extremidade esquerda e outra na extremidade direita, que servem como delimitadores. Um 2AFD aceita sua entrada entrando num especial de parada. Por exemplo, um 2AFD pode reconhecer a linguagem $\{\texttt{a}^n\texttt{b}^n\texttt{c}^n \mid n \ge 0\}$.

- **a.** Seja $A_{\text{2AFD}} = \{\langle M, x\rangle \mid M \text{ é um 2AFD e } M \text{ aceita } x\}$. Mostre que $A_{\text{2AFD}}$ é decidível.
- **b.** Seja $V_{\text{2AFD}} = \{\langle M, x\rangle \mid M \text{ é um 2AFD e } L(M) = \emptyset\}$. Mostre que $V_{\text{2AFD}}$ não é decidível.

### ⬜ 5.21
*2ª ed.: 5.27*

Um ***autômato finito bidimensional*** (AFD-2DIM) é definido da seguinte forma. A entrada é um retângulo $m \times n$, para qualquer $m, n \ge 2$. Os quadrados ao longo da fronteira do retângulo contêm o símbolo # e os quadrados internos contêm símbolos sobre o alfabeto de entrada $\Sigma$. A função de transição é um mapeamento $Q \times \Sigma \longrightarrow Q \times \{\text{E}, \text{D}, \text{C}, \text{B}\}$ para indicar o próximo estado e a nova posição da cabeça (Esquerda, Direita, Cima, Baixo). A máquina aceita quando ela entra em um dos estados de aceitação designados. Ela rejeita se ela tenta mover para fora do retângulo de entrada ou se ela nunca pára. Duas dessas máquinas são equivalentes se elas aceitam os mesmos retângulos. Considere o problema de se testar se duas dessas máquinas são equivalentes. Formule esse problema como uma linguagem, e mostre que ele é indecidível.

### ✅ ★ 5.22
*2ª ed.: 5.28 (Teorema de Rice) — resposta nas p. 226–227*

**Teorema de Rice.** Seja $P$ um problema qualquer sobe máquinas de Turing que satisfaz as duas propriedades abaixo. Como de costume expressamos $P$ como uma linguagem.

- **a.** Para quaisquer MT's $M_1$ e $M_2$, onde $L(M_1) = L(M_2)$, temos $\langle M_1\rangle \in P$ sse $\langle M_2\rangle \in P$. Em outras palavras, a pertinência de uma MT $M$ em $P$ depende somente da linguagem de $M$.
- **b.** Existem MT's $M_1$ e $M_2$, onde $\langle M_1\rangle \in P$ e $\langle M_2\rangle \notin P$. Em outras palavras, $P$ é não-trivial — ela se verifica para algumas, mas não todas, MT's.

Mostre que $P$ é indecidível.

### ⬜ 5.23
*2ª ed.: 5.29*

Mostre que ambas as condições no Problema 5.22 são necessárias para provar que $P$ é indecidível.
