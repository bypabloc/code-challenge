
## Solucion optima 

    const valuesRoman = {
        'I' : 1,
        'V' : 5,
        'X' : 10,
        'L' : 50,
        'C' : 100,
        'D' : 500,
        'M' : 1000,
    }

    var romanToInt = function(s) {
        
        const s_fragmentado = s.split('')
    
        let resultado = 0;
        for( let i = 0; i < s_fragmentado.length; i++ ){
        let value = s_fragmentado[i]
        let valueRoman = valuesRoman[value]
        const value_index_next = parseInt(i) + 1
        const value_next = s_fragmentado[value_index_next]
        if(value_next){
            if( valuesRoman[value_next] > valuesRoman[value] ){
            valueRoman = valuesRoman[value_next] - valuesRoman[value] 
            i = i+1
            }
        }
        resultado = resultado + valueRoman
        }
    
        return resultado
    };

## Resultado:

| Tiempo de ejecución   | Memoria    |
|-----------------------|:-----------|
| 156 ms                | 44.6 MB	 |