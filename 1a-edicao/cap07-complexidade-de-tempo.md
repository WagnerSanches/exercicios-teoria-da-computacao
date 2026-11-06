# Capítulo 7 — Complexidade de Tempo: Exercícios e Problemas (1ª edição)

Sipser, *Uma Introdução à Teoria da Computação*, tradução da 1ª edição (PDF), p. 214–217.

## Resumo

| | Quantidade | Números (1ª ed.) |
|---|---|---|
| **Total** | **23** | Exercícios 7.1–7.11 · Problemas 7.12–7.23 |
| Com resposta na 2ª ed. | 4 | 7.1 (só c, d), 7.2 (só c, d), 7.14, 7.21 |
| **Sem resposta** | **19** | 7.3–7.13, 7.15–7.20, 7.22, 7.23 |

Observação: no 7.1 e no 7.2 a 2ª edição só responde os itens **c** e **d**. Os itens **a, b, e, f** ficam sem resposta.

As respostas ficam em "Soluções selecionadas" do capítulo 7 da **2ª edição** (p. 318–319), com o número da 2ª edição indicado em cada exercício.

Legenda: ✅ = tem resposta na 2ª ed. · ⬜ = sem resposta · ★ = problema mais difícil (marcado com * no livro).

### Correspondência 1ª → 2ª edição

| 1ª ed. | 2ª ed. | Resposta? |
|---|---|---|
| 7.1 | 7.1 | ✅ só c, d |
| 7.2 | 7.2 | ✅ só c, d |
| 7.3 | 7.3 | ⬜ |
| 7.4 | 7.4 | ⬜ |
| 7.5 | 7.5 | ⬜ |
| 7.6 | 7.6 | ⬜ |
| 7.7 | 7.7 | ⬜ |
| 7.8 | — (não aparece na 2ª ed.) | ⬜ |
| 7.9 | 7.8 | ⬜ |
| 7.10 | 7.9 | ⬜ |
| 7.11 | 7.11 | ⬜ |
| 7.12 | 7.12 | ⬜ |
| 7.13 | 7.14 | ⬜ |
| 7.14 | 7.15 | ✅ |
| 7.15 | 7.16 | ⬜ |
| 7.16 | 7.20 | ⬜ |
| 7.17 | 7.17 | ⬜ |
| 7.18 | 7.18 | ⬜ |
| 7.19 | 7.21 | ⬜ |
| 7.20 | 7.13 | ⬜ |
| 7.21 | 7.22 | ✅ |
| 7.22 | 7.24 | ⬜ |
| 7.23 | 7.25 | ⬜ |

---

## Exercícios

### ✅ 7.1 *(só os itens c e d)*
*2ª ed.: 7.1 — resposta na p. 318*

Para cada item abaixo diga se é VERDADEIRO ou FALSO.

- ⬜ **a.** $2n = O(n)$.
- ⬜ **b.** $n^2 = O(n)$.
- ✅ **c.** $n^2 = O(n \log^2 n)$.
- ✅ **d.** $n \log n = O(n^2)$.
- ⬜ **e.** $3^n = 2^{O(n)}$.
- ⬜ **f.** $2^{2^n} = O(2^{2^n})$.

### ✅ 7.2 *(só os itens c e d)*
*2ª ed.: 7.2 — resposta na p. 318*

Para cada item abaixo diga se é VERDADEIRO ou FALSO.

- ⬜ **a.** $n = o(2n)$.
- ⬜ **b.** $2n = o(n^2)$.
- ✅ **c.** $2^n = o(3^n)$.
- ✅ **d.** $1 = o(n)$.
- ⬜ **e.** $n = o(\log n)$.
- ⬜ **f.** $1 = o(1/n)$.

### ⬜ 7.3
*2ª ed.: 7.3*

Quais dos seguintes pares de números são primos entre si? Mostre os cálculos que levaram a suas conclusões.

- **a.** 1274 e 10505
- **b.** 7289 e 8029

### ⬜ 7.4
*2ª ed.: 7.4 (lá o teorema citado é o 7.16)*

Preencha a tabela descrita no algoritmo de tempo polinomial para reconhecimento de linguagem livre-do-contexto do Teorema 7.14 para a cadeia $w = \texttt{baba}$ e a GLC $G$:

$$
\begin{aligned}
S &\to RT \\
R &\to TR \mid \texttt{a} \\
T &\to TR \mid \texttt{b}
\end{aligned}
$$

### ⬜ 7.5
*2ª ed.: 7.5*

A fórmula abaixo é satisfatível?

$$
(x \lor y) \land (x \lor \overline{y}) \land (\overline{x} \lor y) \land (\overline{x} \lor \overline{y})
$$

### ⬜ 7.6
*2ª ed.: 7.6*

Mostre que P é fechada sob união, concatenação, e complemento.

### ⬜ 7.7
*2ª ed.: 7.7*

Mostre que NP é fechada sob união e concatenação.

### ⬜ 7.8
*2ª ed.: não aparece*

Mosre que testar primalidade é solúvel em tempo polinomial se usarmos uma codificação unária ao invés de uma codificação binária para números. Em outras palavras, mostre que a linguagem $PRIMOS\text{-}UNARIOS = \{\texttt{1}^n \mid n \text{ é primo}\}$ está em P.

### ⬜ 7.9
*2ª ed.: 7.8*

Seja $CONEXO = \{\langle G,\rangle \mid \text{é um grafo não-direcionado conexo}\}$. Analise o algoritmo dado na página 145 para mostrar que essa linguagem está em P.

### ⬜ 7.10
*2ª ed.: 7.9*

Um ***triângulo*** em um grafo não-direcionado é um 3-clique. Mostre que $TRIANGULO \in \text{P}$, onde $TRIANGULO = \{\langle G\rangle \mid G \text{ contém um triângulo}\}$.

### ⬜ 7.11
*2ª ed.: 7.11*

Chame os grafos $G$ e $H$ ***isomorfos*** se os nós de $G$ podem ser reordenados de modo que ele fique idêntico a $H$. Seja $ISO = \{\langle G, H\rangle \mid G \text{ e } H \text{ são grafos isomorfos}\}$. Mostre que $ISO \in \text{NP}$.

---

## Problemas

### ⬜ 7.12
*2ª ed.: 7.12*

Seja

$$
EXPMOD = \{\langle a, b, c, p\rangle \mid a, b, c, \text{ e } p \text{ são inteiros em binário tais que } a^b \equiv c \pmod{p}\}.
$$

Mostre que $EXPMOD \in \text{P}$. (Note que o algoritmo mais óbvio não roda em tempo polinomial. Dica: Tente primeiro onde $b$ é uma potência de 2.)

### ⬜ 7.13
*2ª ed.: 7.14*

Mostre que P é fechada sob a operação estrela. (Dica: Sobre a entrada $y = y_1 \cdots y_n$ para $y_i \in \Sigma$, construa uma tabela indicando para cada $i \le j$ se a subcadeia $y_i \cdots y_j \in A^*$ para qualquer $A \in \text{P}$.)

### ✅ 7.14
*2ª ed.: 7.15 — resposta na p. 318*

Mostre que NP é fechada sob a operação estrela.

### ⬜ 7.15
*2ª ed.: 7.16*

Seja $SSOMA\text{-}UNARIO$ o problema da soma de subconjuntos no qual todos os números são representados em unário. Por que a prova de NP-completude para $SOMA\text{-}SUBCONJ$ falha em mostrar que $SSOMA\text{-}UNARIO$ é NP-completa? Mostre que $SSOMA\text{-}UNARIO \in \text{P}$.

### ⬜ 7.16
*2ª ed.: 7.20 (lá as linguagens se chamam CAMMÁX e CAMMIN)*

Suponha $G$ que represente um grafo não-direcionado e seja

$$
CAMINHC = \{\langle G, a, b, k\rangle \mid G \text{ contém um caminho simples de comprimento no máximo } k \text{ de } a \text{ para } b\}.
$$

e

$$
CAMINHL = \{\langle G, a, b, k\rangle \mid G \text{ contém um caminho simples de comprimento no mínimo } k \text{ de } a \text{ para } b\}.
$$

- **a.** Mostre que $CAMINHC \in \text{P}$.
- **b.** Mostre que $CAMINHL$ é NP-completa. Você pode assumir que NP-completude de $CAMHAMILNAOD$, o problema do caminho hamiltoniano para grafos não-direcionado.

### ⬜ 7.17
*2ª ed.: 7.17*

Mostre que, se P=NP então toda linguagem $A \in \text{P}$ exceto se $A = \emptyset$ e $A = \Sigma^*$ é NP-completa.

### ⬜ ★ 7.18
*2ª ed.: 7.18*

Mostre que $PRIMOS = \{n \mid n \text{ é um número primo em binário}\} \in \text{NP}$. (Dica: Para $p > 1$ o grupo multiplicativo $Z_p^* = \{x \mid x \text{ é primo em relação a } p \text{ e } 1 \le x < p\}$ é tanto cíclico quanto de ordem $p - 1$ sse $p$ é primo. Você pode usar esse fato sem prová-lo.

### ⬜ 7.19
*2ª ed.: 7.21*

Seja $DUPLO\text{-}SAT = \{\langle\phi\rangle \mid \phi \text{ tem pelo menos duas valorações que a satisfazem}\}$. Mostre que $DUPLO\text{-}SAT$ é NP-completa.

### ⬜ 7.20
*2ª ed.: 7.13 (lá a linguagem se chama POT-PERM)*

Uma ***permutação*** sobre o conjunto $\{1, \ldots, k\}$ é uma função sobrejetora um-para-um sobre esse conjunto. Quando $p$ é uma permutação, $p^t$ significa a composição de $p$ com ela própria $t$ vezes. Seja

$$
POTENC\text{-}PERM = \{\langle p, q, t\rangle \mid p = q^t \text{ onde } p \text{ e } q \text{ são permutações sobre } \{1, \ldots, k\} \text{ e } t \text{ é um inteiro em binário}\}.
$$

Mostre que $POTENC\text{-}PERM \in \text{P}$. (Note que o algoritmo mais óbvio não roda dentro de tempo polinomial. Dica: Primeiro experimente-o onde $t$ é uma potência de 2).

### ✅ 7.21
*2ª ed.: 7.22 — resposta na p. 318 (a 2ª ed. usa $m$ para o número de nós; aqui é $n$)*

Seja $MEIO\text{-}CLIQUE = \{\langle G\rangle \mid G \text{ é um grafo não-direcionado tendo um subgrafo completo com pelo menos } n/2 \text{ nós, onde } n \text{ é o número de nós em } G\}$. Mostre que $MEIO\text{-}CLIQUE$ é NP-completa.

### ⬜ 7.22
*2ª ed.: 7.24*

Seja $\phi$ uma 3fnc-fórmula. Uma ***≠-atribuição*** às variáveis de $\phi$ é uma na qual cada cláusula contém dois literais com valores-verdade diferentes. Em outras palavras uma ≠-atribuição satisfaz $\phi$ sem atribuir verdadeiro a três literais em nenhuma cláusula.

- **a.** Mostre que a negação de qualquer ≠-atribuição a $\phi$ é também uma ≠-atribuição.
- **b.** Seja $\ne\!SAT$ a coleção de 3fnc-fórmulas que têm uma ≠-atribuição. Mostre que obtemos uma redução em tempo polinomial de $3SAT$ para $\ne\!SAT$ substituindo cada cláusula $c_i$

  $$(y_1 \lor y_2 \lor y_3)$$

  pelas duas cláusulas

  $$(y_1 \lor y_2 \lor z_i) \quad \text{e} \quad (\overline{z_i} \lor y_3 \lor b)$$

  onde $z_i$ é uma nova variável para cada cláusula $c_i$ e $b$ é uma única variável adicional.
- **c.** Conclua que $\ne\!SAT$ é NP-completa.

### ⬜ 7.23
*2ª ed.: 7.25 (lá a linguagem se chama MÁX-CORTE e a dica é mais longa)*

Um ***corte*** em um grafo não-direcionado é uma separação dos vértices $V$ em dois subconjuntos disjuntos $S$ e $T$. O tamanho de um corte é o número de arestas que têm uma extremidade em $S$ e a outra em $T$. Seja

$$
CORTE\text{-}MAX = \{\langle G, k\rangle \mid G \text{ é um corte de tamanho } k \text{ ou mais}\}.
$$

Mostre que $CORTE\text{-}MAX$ é NP-completa. Você pode assumir o resultado do Problema 7.22. (Dica: Mostre que $\ne\!SAT \le_{\text{P}} CORTE\text{-}MAX$.
