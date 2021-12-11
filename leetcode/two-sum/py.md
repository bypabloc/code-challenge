## Solucion optima 

    class Solution:
        def twoSum(self, nums, target):
            d = {}
            for i, n in enumerate(nums):
                m = target - n
                if m in d:
                    return [d[m], i]
                else:
                    d[n] = i
<br>

## Resultado:

| Tiempo de ejecución   | Memoria    |
|-----------------------|:-----------|
| 36 ms                 | 14.4 MB    |
