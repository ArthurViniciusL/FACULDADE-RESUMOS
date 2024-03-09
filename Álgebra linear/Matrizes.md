Classroom: https://classroom.google.com/u/4/c/NjQ4NzQ0MDU5NTAy
Esboço de matriz no LibreOffice Math:
> ```
> left[ matrix{a # b ## c # g} right ]
> ```
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
> Para que seja possível efetuar uma multiplicar uma matriz, o número de colunas de A devem ser iguais ao número de linhas em B.
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
## Matriz inversa 
# Determinantes

# Sistemas lineares