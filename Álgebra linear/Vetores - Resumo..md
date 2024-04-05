Para desenhar um vetor:
```
$$\overrightarrow{vetor}$$
```

Para desenhar a norma:

```
$$\|vetor\|$$
```
Os **vetores** são usados para representar **grandezas** que possuem **direção** e **sentido**, como a força do vento, a velocidade de um carro ou a trajetória de um objeto em movimento.
No plano cartesiano, um vetor é representado por um segmento de reta orientado, ou seja, uma seta que possui **módulo** (comprimento), **direção** e **sentido**.

Um vetor no plano pode ser representado (tratado) de diversas maneiras:
- **Geometricamente:** Por uma seta orientada no plano cartesiano.![[Pasted image 20240401152439.png]]
- **Algebricamente:** Por um par ordenado de números reais (x, y), que representam as coordenadas do ponto final do vetor.

## Norma de um vetor

A norma de um vetor, também conhecida como **módulo** do vetor, é uma medida da sua **"magnitude" ou "tamanho"**. Intuitivamente, podemos pensar na norma como o **comprimento da "seta"** que representa o vetor.

### Exemplo 1:
> Considere um vetor $\overrightarrow{v}$ no plano cartesiano com coordenadas (x, y). A norma de $\overrightarrow{v}$, denotada por $\|\overrightarrow{v}\|$, é calculada pela seguinte fórmula:

$$\|\overrightarrow{v}\| = \sqrt{x^2 + y^2}$$
- **√** representa a raiz quadrada e deve ser realizada depois da entre  $x$ e $y$.
- **x** e **y** são as coordenadas do ponto final do vetor.
### Propriedades da norma
**1. Positividade:** $\|\overrightarrow{v}\|$ ≥ 0 para todo vetor $\overrightarrow{v}$.
**2. Homogeneidade:**  $\|\overrightarrow{tv}\| = \|\overrightarrow{t}\| \|\overrightarrow{v}\|$ para todo escalar $\overrightarrow{t}$ e todo vetor $\overrightarrow{v}$.
**3. Desigualdade Triangular:** ||v + w|| ≤ ||v|| + ||w|| para todos os vetores $\overrightarrow{v}$ e $\overrightarrow{w}$.
**4. Norma do Vetor Zero:** ||0|| = 0, onde **0** é o vetor nulo.
**5. Norma do Vetor Inverso:** ||-v|| = ||v|| para todo vetor $\overrightarrow{v}$.

---
## Operações com vetores no plano

### 1. Igualdade

O vetores $\overrightarrow{u} = (x_1, y_1)$ e $\overrightarrow{v} = (x_2, y_2)$ são iguais se, e somente se, $x_1 = x_2$ e $y_1=y_2$, escrevendo-se $\overrightarrow{u} = \overrightarrow{v}$.

Ou seja, dois ou mais vetores podem ser considerados iguais quando as suas coordenadas são iguais.

Determinar a igualdade de um vetor é necessário em casos onde é necessário determinar:
- **Igualdade de vetores nulos:** O vetor nulo é o único vetor que é igual a si mesmo.
- **Igualdade de vetores opostos:** Se um vetor é o oposto de outro, então os dois vetores são iguais.
#### Exemplo 1:
> Os vetores $\overrightarrow{u} = (3,5)$ e $\overrightarrow{v} = (3,5)$ são iguais.
#### Exemplo 2
> O vetor $\overrightarrow{u} = (x + 1,4)$ é igual ao vetor $\overrightarrow{v} = (5, 2_y - 6)$ se $x + 1 = 5$ e $2_y - 4 = 4$ ou $x = 4$  e $y = 5$. 
> 
> Sendo assim, se $\overrightarrow{u} = \overrightarrow{v}$, então $x = 4$, $y = 5$ e $\overrightarrow{u} = \overrightarrow{v} = (5, 4)$.

----
### 2. Soma
A soma de vetores é representada por: 
$$
\begin{align*}
& \overrightarrow{u} + \overrightarrow{v} = (x_1 + y_1 , x_2 + y_2) \\
& \alpha \overrightarrow{u} = (\alpha x_1, \alpha y_1)
\end{align*}
$$

![[Pasted image 20240402211102.png]]

Ou seja, para que efetuar a soma entre vetores, nós somamos as coordenadas de cada vetor. O que irá resultar em uma nova e única coordenada.

Mas para calcular  soma de um vetor nós usamos:


---
### 3. Subtração (vetor deslocamento)

----
# Vetores no plano (R2)

Vetores no plano sempre vão possuir duas coordenadas, $x$ e $y$, que representam a altura e a largura.
$$
\overrightarrow{A_a}=(x,y)
$$
---
# Vetores no espaço (R3)