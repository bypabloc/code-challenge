## Descripción

Los números romanos están representados por siete símbolos diferentes: &nbsp; <code>I</code>, <code>V</code>, <code>X</code>, <code>L</code>, <code>C</code>, <code>D</code> y <code>M</code>. 

<pre><strong>Simbolo</strong>       <strong>Valor</strong>
I             1
V             5
X             10
L             50
C             100
D             500
M             1000</pre>

Por ejemplo, &nbsp; <code>2</code> se escribe como <code>II</code> &nbsp; en números romanos, solo se suman dos. <code>12</code> está escrito como &nbsp; <code>XII</code>, que es simplemente <code>X + II</code>. El número <code>27</code> se escribe como <code>XXVII</code>, que es <code>XX + V + II</code>.

Los números romanos generalmente se escriben de mayor a menor de izquierda a derecha. Sin embargo, el número de cuatro no es <code>IIII</code>. En cambio, el número cuatro está escrito como <code>IV</code>. Como el uno está antes del cinco, lo restamos haciendo cuatro. El mismo principio se aplica al número nueve, que está escrito como <code>IX</code>. Hay seis casos en los que se usa la resta:

<ul>
    <li> <code>I</code> se puede colocar antes de <code>V</code> (5) y <code>X</code> (10) para hacer 4 y 9. &nbsp; </li>
    <li> <code>X</code> se puede colocar antes de <code>L</code> (50) y <code>C</code> (100) para hacer 40 y 90. &nbsp; </li>
    <li> <code>C</code> se puede colocar antes de <code>D</code> (500) y <code>M</code> (1000) para hacer 400 y 900. </li>
</ul>

Dado un número romano, conviértalo en un número entero.

### Ejemplo 1:
    Entrada: s = "III"
    Salida: 3

### Ejemplo 2:
    Entrada: s = "IV"
    Salida: 4

### Ejemplo 3:
    Entrada: s = "IX"
    Salida: 9

### Ejemplo 4:
    Entrada: s = "LVIII"
    Salida: 58
    Explicación: L = 50, V= 5, III = 3.

### Ejemplo 5:
    Entrada: s = "MCMXCIV"
    Salida: 1994
    Explicación: M = 1000, CM = 900, XC = 90 y IV = 4.

## Restricciones:
<ul>
    <li> <code>1 &lt; = s.length &lt; = 15</code> </li>
    <li> <code>s</code> contiene solo &nbsp; los caracteres <code>('I', 'V', 'X', 'L', 'C', 'D', 'M') </ código>. </li>
    <li> Está <strong> garantizado </strong> &nbsp; que <code>s</code> es un número romano válido en el rango <code>[1, 3999]</code>. </li>
</ul>

<br/>

## Enlace:
[13. Números romanos a entero](https://leetcode.com/problems/roman-to-integer/)

<br/>

### Solución:

- [JavaScript](/leetcode/13.roman-to-Integer/js.md)
- [Python](/leetcode/13.roman-to-Integer/py.md)