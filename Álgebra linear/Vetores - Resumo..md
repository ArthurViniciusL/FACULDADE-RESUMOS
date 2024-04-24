
# Vetores

Seja no plano (R²) ou no espaço (R³) os vetores são _segmentos de retas orientados_ e cada segmento orientado é formado por coordenadas que representam direção, sentido e comprimento. 

Todos os _segmentos orientados_, de mesma direção, mesmo sentido e mesmo comprimento são a representação de um mesmo vetor.

---
### Exemplo 1:
Em um paralelogramo (polígono de quatro lados que possui lados opostos paralelos), os segmentos _AB_ e _CD_ determinam o mesmo vetor $\overrightarrow{v}$.

v = $\overrightarrow{AB} = \overrightarrow{CD}$ 

![[Pasted image 20240403161827.png]]

Quando escrevemos, por exemplo, a notação: v = $\overrightarrow{AB}$ estamos dizendo que  que aquele determinado _segmento orientado_ é de origem $A$ e de extremidade $B$. 

![[Pasted image 20240403164401.png]]

E que também qualquer outro _segmento orientado_ igual a $AB$ é também representante do vetor $\overrightarrow{v}$ .

---
## Norma de um vetor
Sempre que quisermos descobrir o **tamanho de um vetor**, devemos calcular a sua norma.

Quando estamos tratando da norma de um vetor estamos tratando do seu módulo (comprimento). Dizemos que o módulo, a direção e o sentido de um vetor $\overrightarrow{v}$  é também o módulo, a direção e o sentido de qualquer um dos seus representantes. Indica o módulo de v por $\|v\|$.

A norma de um vetor é representada por:
$$\|\overrightarrow{v}\| = \sqrt{x^2 + y^2}$$
- **√** representa a raiz quadrada que deve ser realizada depois da soma entre  $x$ e $y$.
- **x** e **y** são as coordenadas do ponto final do vetor.


----
### Exemplo:
Dado o vetor  $\overrightarrow{v_1} = (-3,4)$, podemos calcular a norma com:

$$
\begin{align*}
||\overrightarrow{v_1}|| = \sqrt{(-3)² + 4^2} \\
= \sqrt{9 + 16} \\
= \sqrt{25} \\
||\overrightarrow{v_1}||= 5
\end{align*}
$$

---
## Propriedades de um vetor

### 1. Soma
A soma de vetores serve para determinar a resultante , o que representa o surgimento de um novo vetor, um vetor resultante.

#### Exemplo
Considerando os vetores u e v que possuem sua soma representada por $\overrightarrow{u} + \overrightarrow{v}$. Vamos escolher um ponto de origem $A$ e traçar o segmento $AB$. Para a partir extremidade $B$ traçar o segmento orientado $BC$ .

![[Pasted image 20240404110924.png]]

Com isso podemos dizer que o vetor de origem $A$ e extremidade $C$ representa a soma de $u$ e$v$.

$\overrightarrow{u} + \overrightarrow{v} = \overrightarrow{AB}$ 
ou
$\overrightarrow{AB} + \overrightarrow{BC} = \overrightarrow{AC}$

**Obs**: Nessa representação não estamos somando as coordenadas do vetor, estamos somando os vetores em si.

---
### 2. Subtração
A subtração de vetores representa a **diferença** entre os segmentos orientado, ou seja, com isso é possível determinar a **distância** e a **direção** entre os pontos.

Considerando dois vetores quais quer, $\overrightarrow{u}$ e $\overrightarrow{v}$, a sua diferença é expressa pela soma entre o vetor $\overrightarrow{v}$ e o oposto do vetor $\overrightarrow{u}$. Ou seja:

$$\overrightarrow{u} = \overrightarrow{AB}$$
$$\overrightarrow{AB} = {B(x_2,y_2)} - {A(x_1,x_2)}$$
**Obs:** Subtração entre as coordenadas dos vetores.

---
### 3. Multiplicação

A multiplicação de um vetor por um escalar é útil para **escalar** a grandeza representada pelo vetor. Por exemplo, se você precisa dobrar a força que está aplicando em um objeto, você pode multiplicar o vetor que representa a força por 2.

### Exemplo
Imagine o vetor $\overrightarrow{v} \neq 0$ e um número real $\alpha \neq 0$. Com isso nós conseguimos obter algo chamado de _produto do número real_ $\alpha$ _pelo vetor_ $\overrightarrow{v}$ . O que resulta em $\alpha \overrightarrow{v}$.

Sendo expresso por:
$$
||\alpha*\overrightarrow{v} = |\alpha| * ||\overrightarrow{v}||
$$
O que por sua vez nós resulta no comprimento de $\overrightarrow{v}$ multiplicado pelo módulo $|\alpha|$. Sendo a direção $\alpha \overrightarrow{v}$  paralelo a  $\overrightarrow{v}$.


**Obs:** Se $\alpha = 0$ ou $\overrightarrow{v} = 0$, já podemos definir que $\alpha \overrightarrow{v} = 0$, porque qualquer coisa multiplicada por zero é igual a zero. 

---
## Tipos de vetores

### 1. Vetores nulos
Quando temos $\|\overrightarrow{v}\| = 0$, ou seja $\overrightarrow{v} = (0,0)$, dizemos que se trata de um vetor nulo.

### 2. Vetor unitário
Se $\|\overrightarrow{v}\| = 1$ então o vetor $\overrightarrow{v}$ é dito unitário

### 3. Vetor unitário W
 Se $\overrightarrow{v}$  for um vetor não-nulo, onde $\|\overrightarrow{v}\| \neq 1$, então podemos dizer que temos o vetor unitário, representado por:  $\overrightarrow{w} = \dfrac{\overrightarrow{v}}{\|\overrightarrow{v}\|}$.
### 4. Vetores perpendicular e ortogonais

Dois vetores são considerados perpendiculares (ortogonais quando estão no $R³$), se o **produto escalar** entre eles for igual a **zero** ($u * v = 0$). Em outras palavras, se o ângulo entre os vetores for de **90°**.

O que é expresso por:  $u \perp v$  -> $u * v = 0$
### 5. Vetores paralelos

Dois vetores são considerados paralelos se eles tiverem a **mesma direção**, podendo ter **sentidos iguais ou opostos**. Então a partir disso dizes que existe um número real $K$ no plano ($k \in \Re$), tal que é possível expressar por:  $u // v$  -> $u = k * v$.

---
## Angulo de um vetor

O angulo formado por dois vetores não-nulos é o Angulo $\theta$  (theta). Mas os vetores forem paralelos ($\overrightarrow{u}//\overrightarrow{v}$) e possuírem o mesmo sentido, então $\theta = 0$
![[Pasted image 20240405153918.png]]

### Representação do cosseno de $\theta$
$$
cos\theta = \dfrac{u*v}{||u|| * ||v||}
$$
### Representação do seno de $\theta$
x

O seno de 0∘ é 0 e o seno de 90∘ é 1.

---
# Vetores no plano
Um vetor é representado por um segmento orientado, ou seja, vão do ponto $A$ até o ponto $B$. Ou seja: $\overrightarrow{v} = \overrightarrow{AB}$

Vetores no plano (R2) sempre vão possuir duas coordenadas, $x$ e $y$, que representam a altura e a largura.

$$
\overrightarrow{A_a}=(x,y)
$$
---
## Operações com vetores no $R^2$
### 1. Soma
A soma dos vetores, ou segmentos orientados, é feita com base na soma entre as coordenadas.

$$
\begin{align*}
AB=(x_1 + x_2, y_1 + y_2) \\ 
\end{align*}
$$
Ou:

$$
\begin{align*}
\overrightarrow{AB} = (x_1, x_2) + (y_1,y_2)
\end{align*}
$$
#### Exemplo:
Soma de vetores.
$$
\begin{align*}
\overrightarrow{u}=(4,1) \\ 
\overrightarrow{v}=(2,6)
\end{align*}
$$

$$
\begin{align*}
&\overrightarrow{u} + \overrightarrow{u}=(4 + 2, 1 + 6) \\
&\overrightarrow{u} + \overrightarrow{u}=(6,7)
\end{align*}
$$

---
### 2. Subtração
A subtração dos vetores, ou segmentos orientados, é feita com base na soma entre as coordenadas.

$$
\begin{align*}
AB=(x_2 - y_2, x_1 - y_1) \\ 
\end{align*}
$$
Ou podemos representar por:

$$
\begin{align*}
\overrightarrow{AB} = (x_1, x_2) - (y_1,y_2)
\end{align*}
$$
---
### 3. Multiplicação
A multiplicação de um vetor é feita entre as coordenadas, por um número real.

$$
\begin{align*}
n*\overrightarrow{u}=(n*x, n*y) \\ 
\end{align*}
$$
#### Exemplo:
Considerando o número real 2. E o vetor $\overrightarrow{u}=(4,1)$. Obtemos:
$$
\begin{align*}
&2 * \overrightarrow{u} = (2*4, 2*1) \\
&2 * \overrightarrow{u} = (8,2)
\end{align*}
$$
![[Pasted image 20240408113353.png]]

----
## Produto escalar

O produto escalar é a multiplicação entre dois vetores que resulta em um valor real.

Sendo definido por:
$$
\begin{align*}
\overrightarrow{u}*\overrightarrow{v} = (x_1 * x_2) + (y_1*y_2)
\end{align*}
$$

---
## Ponto médio
O ponto médio de um vetor no $R^2$ é um ponto que divide o vetor em dois segmentos de igual comprimento. Ou seja, ele está equidistante da origem e da extremidade.
![[Pasted image 20240408114941.png]]

Sendo expresso por:
$$
M= \dfrac{x_1+x_2}{2},\dfrac{y_1+y_2}{2}
$$
--- 
# Vetores no espaço

Vetores no espaço ($R³$), estão lidando co três dimensões. Isso significa que agora cada vetor irá possuir três coordenadas.

$$\overrightarrow{v}= (x,y,z)$$

![[Pasted image 20240408145911.png]]

O que isso implica nas operações? Agora todas operações devem conter a nova coordenada $z$.

## 1. Soma
$$
\begin{align*}
AB=(x_1 + y_1, x_2 + y_2, x_3 + y_3) \\ 
\end{align*}
$$
## 2. Subtração
$$
\begin{align*}
AB=(x_2 - x_1, y_2 - y_1, z_2 - z_1) \\ 
\end{align*}
$$
## 3. Ponto médio

$$
M= \dfrac{x_1+x_2}{2},\dfrac{y_1+y_2}{2}, \dfrac{z_1+z_2}{2}
$$
---

# Produto escalar

O resultado do produto escalar é um **número real**. 

- Para calcular o produto escalar de um vetor no $R²$ usamos:
$$
\overrightarrow{u} * \overrightarrow{v} = (x_1 * x_2) + (y_1 * y_2)
$$
- Para calcular o produto escalar de um vetor no $R³$ usamos:

$$
\overrightarrow{u} * \overrightarrow{v} = (x_1 * x_2) + (y_1 * y_2) + (z_1 * z_2)
$$

---
# Produto vetorial

O produto vetorial é aplicados em vetores no $R³$ e o resultado de um produto vetorial é um **novo vetor**, que é ortogonal aos vetores originais.

O produto vetorial pode ser calculado através uma matriz 3x3. Por isso ele é expresso por:

$$
\begin{align*}
\overrightarrow{u} = (x_1, y_1, z_1) && \overrightarrow{v} = (x_2, y_2, z_2)
\end{align*}
$$

$$
\overrightarrow{u} X \overrightarrow{v} = 
	\begin{bmatrix}
		\overrightarrow{i} &\overrightarrow{j} &\overrightarrow{k} \\
		x_1 & y_1 & z_1 \\
		x_2 & y_2 &z_2
	\end{bmatrix}
$$

E claro, para resolver esse tipo de matriz pode ser usado _Regra de Sarrus_ ou _Teorema de Laplace_.

---
# Produtor misto