## Solucion optima 

    class Solution:
        def romanToInt(self, s: str) -> int:
            values = {
                "I": 1,
                "V": 5,
                "X": 10,
                "L": 50,
                "C": 100,
                "D": 500,
                "M": 1000,
                "IV": 4,
                "IX": 9,
                "XL": 40,
                "XC": 90,
                "CD": 400,
                "CM": 900
            }
            i = 0
            count = 0
            while i < len(s):
                j = i + 1
                if j < len(s) and s[i:j + 1] in values:
                    count += values[s[i:j + 1]]
                    i = j + 1
                else:
                    count += values[s[i]]
                    i += 1
            return count
<br>

## Resultado:

| Tiempo de ejecución   | Memoria    |
|-----------------------|:-----------|
| 52 ms                 | 14.3 MB    |
