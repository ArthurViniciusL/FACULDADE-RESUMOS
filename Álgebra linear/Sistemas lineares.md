O trabalho com equações existe devido à necessidade de encontrarmos valores desconhecidos de incógnitas.

Podemos escrever um sistema de equação de forma matricial. O que chamamos de matriz aumentada.
![[Pasted image 20240322182245.png]]
## Método da eliminação de Gauss.
O método de eliminação de Gauss, também conhecido como método de escalonamento, é um algoritmo eficiente para resolver sistemas de equações lineares. Ele consiste em transformar o sistema original em um sistema equivalente de forma triangular superior, mais fácil de resolver.

### Resolução
**Exemplo:**
$$
\begin{cases}
x + 2y - 3z = 5 \\
2x +y + z = 8 \\
x + 4y - 2z = 12
\end{cases}
$$
#### 1. Criar uma matriz aumentada com os elementos.
$$
\begin{bmatrix}
1 & 2 & -3 & | & 5 \\
2 & 1 & 1 &| & 8 \\
1 & 4 & -2 & | & 12
\end{bmatrix}
$$
---
#### 2. Selecionar a diagonal principal.

	![[Pasted image 20240326194240.png]]

---
#### 3. Aplicando o método de escalonamento.
Vídeo aula de referência: https://www.youtube.com/watch?v=E5AqlJutoVo&t=573s

Também chamado de eliminação de Gauss. O método de eliminação deve ser aplicada até que **todos os elementos abaixo da diagonal principal estejam zerados**.
![[Pasted image 20240326194912.png]]

Para aplicar escalonamento devemos seguir os seguintes passos:
##### 3.1. Verifique se o elemento na primeira coluna é diferente de zero.
Se sim, troque a primeira linha com a linha que contém o primeiro elemento diferente de zero. Isso garante que você tenha um coeficiente principal diferente de zero na primeira linha.

---
##### 3.3. Definir o elemento multiplicador geral da linha.
O multiplicador da linha $M_L$ deve ser usado nos outros elementos da linha em que ele multiplica. O multiplicador pode ser qualquer número que possibilite zera o primeiro elemento da linha 2 em diante.

No nosso caso um número que serve como multiplicador é o 2 na linha 1.
$$
M_L = 2
$$

----

##### 3.4. Definir a operação para anular a linha.

A estrutura básica nessa parte é:
$$M_L * L_1 - L_2$$
 
A primeira condição é analisar se o multiplicador da linha é positivo ou negativo. Caso ele seja negativo, então deve ser aplicado uma operação de adição entre as linhas. Caso seja positivo, uma operação de subtração.

Como nosso $M_L$ é positivo, vamos utilizar uma operação de subtração entre $L_1$ e $L_2$.

Outro ponto é que (caso seja necessário para fazer a anulação da linha acontecer), a linha 2 também pode receber um multiplicador.

---
##### 3.5. Atualizando a linha 2.

Seguindo operação: $2*L_1 - L_2$.
$$\begin{align*}
&a_{2,1} = 2 * 1 - 2 \\
&a_{2,2} = 2 * 2 - 1 \\
&a_{2,3} = 2 * (-3) - 1 \\
&a_{2,4} = 2 * 5 - 8
\end{align*}
$$
**Obtemos**:
$$a_{2,j} = \begin{bmatrix} 0 &3 &-7 &2 \end{bmatrix}$$

----

##### 3.5. Atualizando a linha 3.

Na linha 3 conseguimos visualizar que não é necessário um multiplicador para que seja possível zerar $L_{3,1}$. Pois os elementos de $L_{1,1}$ e $L_{3,1}$ são iguais.

Seguindo a operação: $L_{1} - L_{3}$.
$$\begin{align*}
&a_{3,1} = 1 - 1 \\
&a_{3,2} = 2 - 4 \\
&a_{3,1} = (-3) + 2 \\
&a_{3,1} = 5 - 12
\end{align*}
$$

**Obtemos:**

$$a_{3,j}=\begin{bmatrix}0 &-2 &-1 &-7\end{bmatrix}$$

---
##### 3.5. Montar a nova matriz.
A matriz resultante foi a seguinte:
$$
\begin{bmatrix}
1 &2 &-3 &| &5 \\
0 &3 &-7 &| &2 \\
0 &-2 &-1 &| &-7
\end{bmatrix}
$$
Infelizmente ela ainda não foi finalizada, observe que ainda temos um elemento abaixo da diagonal principal que não foi zerado.
![[Pasted image 20240328150500.png]]
Isso significa que o nosso objetivo **ainda não foi concluído, então devemos continuar aplicando o método de escalonamento**.

----
##### 3.6. Reaplicando o método.
Como não é mais necessário zerar elementos na $L_2$ então só vamos observar os elementos da $L_3$.

Primeira coisa a ser feita é escolher um novo multiplicador para zerar o elemento abaixo da diagonal principal.  Nessa nova matriz será necessário inserir um multiplicador para em $L_3$.

$M_{L2} = 2$.
$M_{L3} = 3$.

A operação escolhida será uma soma, pois conseguimos zerar o elemento $-2$.

Seguindo a operação: $M_{L2}*L_2+M_{l3}*L_3$

$$
\begin{align*}
&a_{3,1} = 0\\
&a_{3,2} = 2 * 3 + 3*(-2)\\
&a_{3,3} = 2 * (-7) + 3 * (-1)\\
&a_{3,4} = 2 *2 + 3 * (-7)
\end{align*}
$$

**Obtemos:**

$$
a_{3,j} = 
\begin{bmatrix}
0 &0 &-17 &-17
\end{bmatrix}
$$
----
##### 3.7. Finalizando a matriz.

Agora que conseguimos zerar todos os elementos abaixo da diagonal principal então podemos de fato construir a matriz.
$$
\begin{bmatrix}
1 &2 &-3 &| &5 \\
0 &3 &-7 &| &2 \\
0 &0 &-17 &| &-17
\end{bmatrix}
$$

----
#### 4. Montando o novo sistema linear.
$$
\begin{cases}
x + 2y - 3z = 5 \\
3y - 7z = 2 \\
-17z = -17
\end{cases}
$$

A primeira coisa que podemos observar é que temos menos variareis para resolver. E para facilitar ainda mais o trabalho de resolução, podemos começar a resolver o sistema de baixo para cima.

---
#### 5. Resolver o sistema.
##### 5.1. Obtendo o valor de Z.

Além de $Z$  não temos mais nenhuma variável significa que já podemos isolá-lo e resolver o sistema.

$$
\begin{align*}
-17z = -17 \\
Z = \dfrac{-17}{-17} \\
Z = 1
\end{align*}
$$
---
##### 5.2. Obtendo o valor de Y.
Como já conseguimos obter o valor de $Z$ então podemos começar a substitui-lo no nosso sistema.

$$
\begin{align*}
3y -7*1 = 2 \\
3y -7 = 2 \\
\end{align*}
$$

Agora vamos isolar tudo que está depois de $Y$, invertendo o sinal.

$$
\begin{align*}
3y = 2 + 7 \\
3y = 9
\end{align*}
$$

Agora isolamos $Y$ para obter o seu valor.
$$
\begin{align*}
3y = 2 + 7 \\
y = \dfrac{9}{3} \\
y = 3
\end{align*}
$$
---
##### 5.3. Obtendo o valor de X.
Já conseguimos obter os valores de $Y$ e $Z$, o que nos possibilita resolver o sistema para obter o valor de $X$.
$$
\begin{align*}
x + 2*3 - 3*1 = 5 \\
x + 6 - 3 = 5 \\
x = 5 - 6 + 3 \\
x = 2
\end{align*}
$$
---
## Classificação dos sistemas lineares.
## Classificação de Sistemas Lineares

Os sistemas lineares são classificados em três tipos, de acordo com o número de soluções que possuem:

1. **Sistema Possível Determinado (SPD):** possui **uma única solução**. Isso ocorre quando o número de equações é igual ao número de variáveis e o determinante do sistema é diferente de zero (D ≠ 0).

2. **Sistema Possível Indeterminado (SPI):** possui **infinitas soluções**. Isso ocorre quando o número de equações é menor que o número de variáveis e o determinante do sistema é igual a zero (D = 0). Nesse caso, o sistema possui uma variável livre, que pode assumir qualquer valor real.

3. **Sistema Impossível (SI):** **não possui soluções**. Isso ocorre quando o número de equações é maior que o número de variáveis e o determinante do sistema é diferente de zero (D ≠ 0). Nesse caso, as equações do sistema são incompatíveis entre si.
---
### O que determina a classificação de um sistema linear

- **Número de equações:** O número de equações determina o número de relações entre as variáveis.
- **Número de variáveis:** O número de variáveis determina o número de incógnitas no sistema.
- **Determinante do sistema:** O determinante do sistema é um número que indica se o sistema possui solução única, infinitas soluções ou nenhuma solução.
---
### Como determinar a classificação de um sistema linear.

1. **Verifique o número de equações e variáveis.**
2. **Calcule o determinante do sistema.**
3. **Compare o determinante com zero e o número de equações com o número de variáveis.**
---
### Exemplo

Considere o sistema linear:

```
x + y = 2
2x + 2y = 4
```

- **Número de equações:** 2
- **Número de variáveis:** 2
- **Determinante do sistema:** D = 0

**Classificação:** Sistema Possível Indeterminado (SPI).

**Explicação:**
- O sistema possui duas equações e duas variáveis, ou seja, o número de equações é igual ao número de variáveis.
- O determinante do sistema é igual a zero.
- Como o número de equações é igual ao número de variáveis e o determinante é igual a zero, o sistema possui infinitas soluções.