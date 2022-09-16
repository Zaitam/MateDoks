---
title: "Permutacion"
description: ""
draft: false
images: []
---

Una permutacion es la variacion del orden de los elementos de una lista. 
Por ejemplo: $[A, B, C]$ y $[B, C, A]$ son permutaciones de $[B, A, C]$, pero $[B,B,A]$ no lo es.
Es similar a los Anagramas

### Factorial
Nos permite contar la cantidad de permutacione que tenemos una lista. Su notacion es de:
$$x! = 1\times2\times3\times4\times5\dots\times(x-1)\times x $$

Para contar las permutaciones de una lista con **items unicos**, es decir, que no se repiten, podemos hacer factorial de la longitud de la lista:
$Lista = 1;2;3;4;5;6;7$
La cantidad de elementos de la lista es 7, entonces tenemos $7! = 1\times2\times3\times4\times5\times6\times7 = 5040$

### Factorial con repeticion
Si la lista contiene elementos repetidos, no podemos hacer $!x$ ya que $[A_{1},B,A_{2}]$ (Ignorardo los sub-indices) es igual a $[A_{2},B,A_{1}]$.

Para sacar estos casos hay que dividir el factorial por la cantidad de items repetidos factorial. Entonces $[A,B,A]$ es igual a:
$$\frac{3!}{2!}=\frac{3\times2\times1}{2\times1}=3$$
Ahora en una lista con multiples repetidos, no incrementamos la division, sino que multiplicamos el denominador por el factorial de la nueva cantidad del numero repetido. Es decir que para $[A,A,B,B]$ tenemos:
$$\frac{4!}{2!\times2!}=\frac{4\times3\times2\times1}{(2\times1)\times(2\times1)}=\frac{24}{4}=6$$
