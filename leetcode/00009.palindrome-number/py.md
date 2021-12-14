## Solucion optima 

    class Solution:
        def isPalindrome(self, x: int) -> bool:
            x = str(x)
            
            if x[0] != x[-1]:
                return False
            elif len(x) <= 2 and x[0] == x[-1]:
                return True
            else:
                return self.isPalindrome(x[1:-1])
<br>

## Resultado:

| Tiempo de ejecución   | Memoria    |
|-----------------------|:-----------|
| 60 ms                 | 14.2 MB    |
