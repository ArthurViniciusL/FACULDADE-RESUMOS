**A** combinação é uma expressão construída a partir de um **conjunto de _termos_, multiplicando cada termo por uma _constante_**. O conceito de combinações lineares é central para a álgebra linear e campos relacionados da matemática.

Com isso podemos definir que seja $v_1, v_2, v_3, ... v_n$ o conjunto de vetores $v$ de um espaço vetorial $V$ ($R²$ ou $R³$), onde $a_1, a_2, a_3... a_n$ são os números reais. E se $v$ pertence ($\in$) a $V$ tal que $v = a_1*v_1 + a_2*v_2 + a_3 * v_3$ ... $+ a_n * v_n$ , então $v$ é dito uma combinação linear de $v_1, v_2, v_3, ..., v_n$.

$$
\begin{align*}
\overrightarrow{w} = {a_1 * \overrightarrow{u}} + {a_2 *\overrightarrow{v}} ...
\end{align*}
$$
### Observações
-  $a_n$ também pode ser representado por: a, b, c,... z.

## Exemplo 1:
Dados os vetores $\overrightarrow{u}=(2,-3,2)$ e $\overrightarrow{v}=(-1,2,4)$ no R³, mostre que $\overrightarrow{w}=(7,-11,2)$ é a combinação linear de $\overrightarrow{u}$ e $\overrightarrow{v}$.
![[exemplo_1.png]]
### Observações
- A primeira coisa a ser feita é multiplicar o número pela coordenada do vetor e para isso, cada vetor terá um número real associado a ele.
- A ordem de resolução dos sistemas não importa muito, desde que todas as incógnitas sejam descobertas.
- O sistema linear só pode ser dado como resolvido, quando todas as incógnitas tiverem sido isoladas.
- Observe que eu comecei resolvendo o sistema A para descobrir $a_2$, segui para o sistema B e descobri $a_1$. E a partir disso pude voltar para o sistema A e realizar a substituição de $a_1$.
### Exemplo 2:
Seja o espaço vetorial $M(2*2)$ e os vetores:
$$
{\overrightarrow{v}_1} = \begin{bmatrix}
1 & 0 \\
1 & 1
\end{bmatrix}
\
{\overrightarrow{v}_2} = \begin{bmatrix}
-1 & 2 \\
0 & 1
\end{bmatrix}
\
{\overrightarrow{v}_3} = \begin{bmatrix}
0 & -1 \\
2 & 1
\end{bmatrix}
$$
Escreva o vetor $\overrightarrow{v}$:
$$
\overrightarrow{v} = \begin{bmatrix}
1 & 8 \\
0 & 5
\end{bmatrix}
$$
Como a combinação linear entre $\overrightarrow{v}_1$, $\overrightarrow{v}_2$ e $\overrightarrow{v}_3$.
![[exemplo_2.png]]

---
# Vetores Li e Ld.

Na definição geral dizemos que se o conjunto de vetores $A = \{v_1, v_2, v_3,..., V_n\}$ $\subset$ $V$ e $a_1, a_2, a_3, ..., a_n$  $\in$ $\Re$ . Com isso, se a equação: $a_1*v_1+a_2*v_2+a_3*v_3 + ... + a_n * v_n = 0_v$. admite que a única solução seja: $a_1=0$, $a_2=0$, $a_3=0$, ..., $a_n=0$, então o conjunto $A$ é linearmente dependente, caso contrário, $A$ linearmente dependente.

- $\subset$ : Contém.
- Se o resultado de todas as _incógnitas forem iguais a zero então o vetor é Linearmente independente_, mas caso uma das _incógnitas forem diferente de zero_, então o _vetor é linearmente dependente_.
## Vetores Li
Um conjunto de vetores é dito _linearmente independentes_ são se um ou mais vetores puderem ser escritos como uma combinação linear dos demais.

### Exemplo 1:
Verifique se o conjuntos abaixo é Li ou Ld.
![[exemplo_3_1.png]]
![[exemplo_3_2.png]]
Todas nossas incógnitas resultaram em zero.

## Exemplo 2:

## Vetores Ld
Um conjunto de vetores é dito _linearmente independente_ se nenhum vetor puder ser escrito como uma combinação linear dos demais.
![[exemplo_4.png]]
### Exemplo 1:
Verifique se o conjuntos abaixo é Li ou Ld.
![[exemplo_5-1.png]]
![[exemplo_5_2.png]]

---
# Base e dimensão.
Assumimos que o conjunto $B={v_1,v_2,v_3,..., v_n}$ $\subset$ $V$ contem uma base $V$ se:
1. B for linearmente independente;
2. E o conjunto B gerar um um espaço vetorial $V$.

Para auxiliar essa trabalhos podemos usar o teorema que define que: Se $V$ possui uma base com $n$ vetores, então a dimensão de $V$ é igual a $n$, ou seja: 

$$
dimV = n
$$
### Exemplo 1:
Sabendo que $dimR² = n$, $dimP_n = n + 1$ e $dimM_{mxn} = m*n$. Mostre que:
$B = \{(2,1,-1), (-1,0,1), (0,0,1)\}$$ é uma base do $R³$.

![[Álgebra linear/exemplo_6_1.png]]![[Álgebra linear/exemplo_6_2.png]]

---
# Transformação Linear.
Transformação linear é um tipo particular de função entre dois espaços vetoriais que preserva as operações de adição vetorial e multiplicação por escalar.

Seja $V$ (R²) e $W$ (R³) dois espaços vetoriais. Uma aplicação $T : V \rightarrow W$ é dita uma transformação linear se:
1. $T_{(u+v)} =  T_{(u)} + T_{(v)} \forall_{u,v} \in V$
2. $T_{(a*u)} = a*T_{(u)} \forall_{u,v} \in V$ e $a \in \Re$
- **Obs:**
	- A transformação é nula se o espaço vetorial for nulo: $T{0_{W}} = 0_W$
	- A transformação vetorial é resultado da multiplicação entre um número real e um vetor: $T_{(a_1 * V_1 + a_2 * V_2 + a_3 * V_3 ... a_n * V_n)} = a_1 * T_{(V1)} + a_2 * T_{(V2)} + a_3 * T_{(V3)} .... a_n * T_{(Vn)}$

### Exemplo 1:
![[exemplo_7.png]]