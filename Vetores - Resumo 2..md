
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
$$\overrightarrow{u} +  (-\overrightarrow{v})$$
Exemplo de Vetores opostos:
![[Pasted image 20240404231410.png]]

#### Exemplo
A diferença de dois vetores u e v quaisquer é o vetor $\overrightarrow{u} + (-\overrightarrow{v})$. Sejam os vetores $\overrightarrow{u}$ e $\overrightarrow{v}$ representados pelos segmentos orientados $AB$ e AC, respectivamente. Construído o paralelogramo $ABCD$, verifica-se que a soma $\overrightarrow{u} + \overrightarrow{v}$ é representada pelo segmento orientado $AD$
(uma das diagonais) e que a diferença $\overrightarrow{u} - \overrightarrow{v}$ é representada pelo segmento orientado $CB$ (a outra
diagonal).

![[Pasted image 20240404203327.png]]

Quando os vetores estão aplicados no mesmo ponto, pode se verificar que, por exemplo, a diferença $\overrightarrow{u} - \overrightarrow{v}$ tem origem na extremidade de $\overrightarrow{v}$ (e, por conseguinte, a diferença $\overrightarrow{u} -\overrightarrow{v}$ tem origem na extremidade de $\overrightarrow{u}$ ).

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
### 4. Vetores perpendicular
O que é expresso por:  $u \perp v$ ;

Dois vetores são considerados ortogonais se o **produto escalar** entre eles for igual a **zero** ($u * v = 0$). Em outras palavras, se o ângulo entre os vetores for de **90°**.
### 5. Vetores paralelos
O que é expresso por:  $u // v$ ;

Dois vetores são considerados paralelos se eles tiverem a **mesma direção**, podendo ter **sentidos iguais ou opostos**. Então a partir disso dizes que existe um número real $K$ ($k \in \Re$), tal que é possível expressar por $u = k * v$.

---
## Angulo de um vetor

O angulo formado por dois vetores não-nulos é o Angulo $\theta$  (theta). Mas os vetores forem paralelos ($\overrightarrow{u}//\overrightarrow{v}$) e possuírem o mesmo sentido, então $\theta = 0$
![[Pasted image 20240405153918.png]]

O que é representado por:
$$
cos\theta = \dfrac{u*v}{||u|| * ||v||}
$$

---
# Vetores no plano
# Produto escalar
# Produto vetorial
# Vetores no espaço
# Produtor misto