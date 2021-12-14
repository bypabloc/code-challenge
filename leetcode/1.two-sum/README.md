## Descripción

Dada una matriz de números enteros (<code>nums</code>) y un número entero (<code>target</code>), devuelve índices de los dos números de manera que se sumen al objetivo.

Puede suponer que cada entrada tendría exactamente una solución y no puede usar el mismo elemento dos veces.

Puede devolver la respuesta en cualquier orden.

### Ejemplo 1:
    Entrada: nums = [2,7,11,15], target = 9
    Salida: [0,1]
    Salida: Porque nums[0] + nums[1] == 9, retornamos [0,1].

### Ejemplo 2:
    Entrada: nums = [3,2,4], target = 6
    Salida: [1,2]
    Salida: Porque nums[1] + nums[2] == 6, retornamos [1,2].

### Ejemplo 3:
    Entrada: nums = [3,3], target = 6
    Salida: [0,1]
    Salida: Porque nums[0] + nums[1] == 6, retornamos [0,1].

## Restricciones:
- 2 <= nums.length <= 10<sup>4</sup>
- -10<sup>9</sup> <= nums[i] <= 10<sup>9</sup>
- -10<sup>9</sup> <= target <= 10<sup>9</sup>
- <strong>Solo existe una respuesta válida.</strong>

## Seguimiento:
¿Puede idear un algoritmo que sea menos complejo que el tiempo? O(n2) 
<br/>

## Enlace:
[LeetCode -> two sum](https://leetcode.com/problems/two-sum/)

<br/>

### Solución:

- [JavaScript](/leetcode/1.two-sum/js.md)
- [Python](/leetcode/1.two-sum/py.md)