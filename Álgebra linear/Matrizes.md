Classroom: https://classroom.google.com/u/4/c/NjQ4NzQ0MDU5NTAy
Esboço de matriz no LibreOffice Math:
> ```
> left[ matrix{a # b ## c # g} right ]
> ```

Exemplo de matriz para Markdown
```
$$X = \begin{bmatrix}
1 & x_{1}1 & x_{2} \\
1 & x_{3} 1 & x_{4}
\end{bmatrix}$$
```

$$X = \begin{bmatrix}
1 & x_{1}1 & x_{2} \\
1 & x_{3} 1 & x_{4}
\end{bmatrix}$$


# Matrizes

Uma matriz é uma estrutura de tabela composta por _m_ linhas e _n_ colunas, com uma ordem _m_ x _n_. Onde _m_ e _n_ devem ser maior ou diferentes de zero.

- Letra **i** a representação para a posição do valor linha.
- Letra **j** a representação para a posição do valor coluna.

--- 
## Matriz quadrada
Uma matriz é considerada quadrada quando a quantidade linhas é igual a quantidade de colunas. Ou seja, ela é de ordem _n_.

![[Pasted image 20240304130301.png]]

![[Pasted image 20240304132331.png]]

Sempre que uma matriz for quadrada então ela irá possuir duas diagonais, a principal e a secundária.

### Diagonal principal
> Sempre vai ser representando da esquerda para a direita.
> ![[Pasted image 20240304160854.png]]
### Diagonal secundária
> Sempre vai ser representada da direita para a esquerda.
> ![[Pasted image 20240304161026.png]]
> ---- 
## Matriz identidade
Uma matriz pode ser assumida como identidade quando todos os elementos da sua _digonal principal_ são iguais ao _valor 1_ e os _outro elementos são iguais a 0_.

![[Pasted image 20240304130301.png]]

----
## Operações com matrizes
### Adição
> Para ser possível somar matrizes é importante que elas _sejam de mesma ordem_.
>
> Para somar os elementos de uma matriz, devemos somar os elementos correspondentes em cada linha e em cada coluna.
>
> Então por exemplos temos:
>
> ![[Pasted image 20240304171439.png]]
>
> ![[Pasted image 20240304171506.png]]
>
> O que resulta em uma operação assim:
>
> ![[Pasted image 20240304172529.png]]
>
> Sendo assim construída uma nova matriz de ordem 2:
>
> ![[Pasted image 20240304172758.png]]
> --- 
### Subtração
> A subtração de matrizes segue a mesma lógica da adição, ou seja, eu realizo a minha operação sobre os indicies correspondentes.
> 
> Pegando as matrizes A e B como exemplo, temos:
> 
> ![[Pasted image 20240304175143.png]]
> O que gera a matriz:
> ![[Pasted image 20240304175403.png]]
### Multiplicação
> Para que seja possível efetuar uma multiplicar uma matriz, o número de colunas de A devem ser iguais ao número de linhas de B.
> 
> **Exemplo:**
> ![[Pasted image 20240309202327.png]]
> ![[Pasted image 20240309202359.png]]

> Para efetuar a multiplicação entre os elemento de uma matriz devemos multiplicar o valor da coluna A, pelos elementos da linha em B. E em seguida somar o resultado de cada multiplicação para que seja gerado o elemento da matriz AxB.
> **Exemplo:**
> ![[Pasted image 20240308182225_1.png]]
> ![[Pasted image 20240308182225_2.png]]
> ![[Pasted image 20240308182225_3.png]]

> **Primeira linha da matriz**
> ```
> i1xj1 : A.B = (1 x 1) + (2 x 2) = 5
> i1xj2 : A.B = (1 x -2) + (2 x 4) = 6
> i1xj3 : A.B = (1 x 3) + (2 x 0) = 3
> ```

> **Segunda linha da matriz**
> ```
> i2xj1 : (3 x 1) + (-1 x 2) =  1
> i2xj2 : (3 x -2) + (-1 x 4) = -10
> i2xj3 : (3 x 3) + (-1 x 0) = 9
> ```

 
> **O resultado da matriz então é:** 
> ![[Pasted image 20240309201531.png]]

### Divisão
> Não existe.

---

# Determinantes

O determinante de uma matriz é importante para várias aplicações, como verificar se três pontos estão alinhados no plano cartesiano, calcular áreas de triângulos, resolver sistemas lineares, entre outras aplicações na matemática.

O determinante é uma função matemática que associa a cada matriz quadrada um número real. Este número é **calculado a partir dos elementos da matriz** e possui propriedades específicas que o tornam uma ferramenta poderosa na resolução de problemas matemáticos.
## Determinante de ordem 1
- Para matrizes de ordem 1, o determinante é igual ao seu único elemento.
## Determinante de ordem 2
- Para matrizes de ordem 2, o determinante é calculado pela diferença (subtração) entre o produto dos termos da diagonal principal e os termos da diagonal secundária. Ou seja **diagonal principal - diagonal secundária**.
- **Exemplo:**
> $$A = \begin{bmatrix}
{4} & {2} \\
{1} & {1}
\end{bmatrix}$$
> $$
 \begin{align*} d_1 & = 4 * 1 \\ d_2 & = 2 * 1 \\ D & = (4 - 2) => 2 \end{align*}
$$

## Determinante de ordem 3 (regra de Sarrus)
- Para matrizes de **ordem 3**, utiliza-se a **regra de Sarrus**. A Regra de **Sarrus** é um método prático usado para calcular o determinante de uma matriz quadrada de ordem.
- **Exemplo:**
	Aqui estão os passos para **aplicar a Regra de Sarrus**:
1. Repita as duas primeiras colunas ao lado da matriz;
	![[Pasted image 20240319203214.png]]
	![[Pasted image 20240319203236.png]]
2. Multiplique os valores de todas as **diagonais da principais**;
	![[Pasted image 20240320111940.png]]
	$$ \begin{align*}
	1 . 5 . 8 = 40 \\
	2 . 6 . 2 = 24 \\
	3 . 2 . 5 = 30 \\
	 \end{align*}$$
3. Multiplique os valores de todas as **diagonais secundárias**;
	![[Pasted image 20240320112254.png]]

$$ \begin{align*}
2 . 2 . 8 = 32 \\
1 . 6 . 5 = 30 \\
3 . 5 . 2 = 30 \\
 \end{align*}$$
4. Some os resultados das multiplicações das diagonais do mesmo sentido;
	$$\begin{align*}
	d_1 = 40 + 24 + 30 => 94 \\
	d_2 = 32 + 30 + 30 => 92 \\
	\end{align*}$$
5. Subtraia os dois valores finais para obter a determinante.
$$
	\begin{align*}
	&Det = d_1 - d_2  \\ &Det = 2
	\end{align*}
$$
## Determinante de ordem ≥ 4 (Teorema de Laplace)
O **Teorema de Laplace** é um método para **calcular o determinante de matrizes** quadradas de ordem _n_. Normalmente, é utilizado quando as matrizes são **de ordem igual ou maior que 4**.

Para usar o Teorema de Laplace é necessário obter o cofator de cada índice da matriz.


### **Como funciona o teorema de Laplace.**
No teorema de Laplace a **determinante** da matriz será o produto da soma entre os elemento multiplicados pelos seus cofatores.

![[Pasted image 20240320224332_1.png]]
1. Selecione uma fila (linha ou coluna), da matriz (Quanto mais zeros houver na fila, melhor para facilitar o cálculo);
![[Pasted image 20240320224332_3.png]]
2. Multiplicar cada elemento pelo **cofator** do valor no índice;
	[[Matrizes#**Como descobri o cofator.**]]
 
 $$\begin{align*}
&a_{4,4} = Fila * c{i,j} \\
&a_{4,4} = 0 * c_{1,3} => 0 \\
&a_{4,4} = 3 * c_{2,3} => ? \\
&a_{4,4} = 0 * c_{3,3} => 0\\
&a_{4,4} = 1 * c_{4,3} => ?
\end{align*}$$

$$\begin{align*}
&c_{2,3} = 0 * 7 => 21 \\
&c_{4,3} = 1 * 13 => 13 \\
\end{align*}$$
3. Somar o resultado da multiplicação entre cada elemento.
$$\begin{align*}
&c_{2,3} + c_{4,3} = 21 + 13 \\
&D = 34
\end{align*}$$
### **Como descobri o cofator.**
$$
c_{i,j} = (-1)^{i+j} . M_{i,j} 
$$
> Cofator é um número associado a um elemento qualquer de uma matriz quadrada.
> O cofator deve ser obtido de cada elemento da matriz.

1. Somar os índices de i + j;
$c_{2,3}=(-1)^{2+3} => 5$
$c_{4,3}=(-1)^{4 + 3} => 7$
2. Calcular os determinantes;
 **Exemplo:**
 - Exclua a linha e coluna do seu cofator da matriz principal.
 > $c_{2,3}=?$
 > ![[Pasted image 20240320224332_2.png]]
  
- Gere uma nova matriz com os outros valores.
 > ![[Pasted image 20240320234222.png]]
 > Como essa se trata de uma matriz 3x3 então a regra de **Sarraus** será usada.
 >
- Determinante.
> $c_{2,3}=-7$
> Repita o mesmo processo para os outros índices.

3. Aplicar a formula;
$$\begin{align*}
&c_{2,3} = (-1)^{5} * (-7) \\
&c_{2,3} = 7 \\
\end{align*}$$
$$
\begin{align*}
&c_{4,3} = (-1)^{7} * (-13) \\
&c{4,3} = 13
\end{align*}
$$
5. Voltar para o teorema de **Laplace**.


**Obs:**
- Se $(-1)^{i+j}$ sendo for impar, o resultado é = -1;
- Se $(-1)^{i+j}$ sendo for par, o resultado é = 1;
- M representa a determinante do cofator.

---
# Matriz inversa
Uma matriz inversa é uma matriz quadrada ($A$) que quando multiplicada por sua matriz inversa ($A^{-1}$), resulta em uma matriz identidade. Tal que $A*A^{-1}=I_{n,j}$ .

**Exemplo:**
![[Pasted image 20240321175723.png]]

- Encontrar o determinante da matriz ([[Determinantes]]);
$D = 2$
- Dividir os valores pelo determinante;
![[Pasted image 20240321175723_2.png]]
![[Pasted image 20240321180535.png]]
- Inverter os elementos da diagonal principal (permutar).
![[Pasted image 20240321180725.png]]

- Inverte os **sinais** da diagonal secundária.
![[Pasted image 20240321181048.png]]

E o resultado final da matriz inversa é:
![[Pasted image 20240321181320.png]]

# Sistemas lineares
O trabalho com equações existe devido à necessidade de encontrarmos valores desconhecidos de incógnitas.

https://www.todamateria.com.br/sistemas-lineares/

Podemos escrever um sistema de equação de forma matricial. O que chamamos de matriz aumentada.
![[Pasted image 20240322182245.png]]
## Método da eliminação de Gauss
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
**1. Criar uma matriz aumentada.**
$$
\begin{bmatrix}
1 & 2 & -3 & | & 5 \\
2 & 1 & 1 &| & 8 \\
1 & 4 & -2 & | & 12
\end{bmatrix}
$$
**2. Selecionar a diagonal principal.**
![[Pasted image 20240326194240.png]]

**3. Aplicando a eliminação de Gauss.**
O método de eliminação deve ser aplicada até que **todos os elementos abaixo da diagonal principal estejam zerados**.
![[Pasted image 20240326194912.png]]

Outra regra é que 

A estrutura do **algorítimo** deve seguir os seguintes passos:
- 1. Algumas coisa sobre o zero no primeiro elemento
x
- 2. Encontrar o número pivô.
x
pivô = elemento linha acima
- 3. x

multiplicador = (elemento linha atual / pivô)
elemento linha atual - multiplicador * elemento linha pivô
**4. Resolver o sistema.**
x
jogar os valores pós variável para o outro lado e inverter o sinal
resolver o sistema
isolar a varivel
na hora de dividir não inverte o sinal

Os coeficientes são os números que multiplicam as letras, chamadas de incógnitas, que nos sistemas lineares, possuem expoente no máximo igual a 1.

## Classificação dos sistemas lineares