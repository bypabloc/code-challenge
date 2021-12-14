
## Solucion optima 

    const twoSum = (nums, target) => {
        // creamos un objeto para mapear los valores, "valor: indice"
        let map = {}
        
        // llenamos el mapa
        for(i in nums){
            map[nums[i]] = i;
        }

        // recorremos el array para comparar cada valor
        for(i in nums){
            // Aca obtenemos un primer elemento Ejemplo: - [2,7,11,15], target = 9
            const num = nums[i]; // obtendre un 2 
            const residue = target - num; // calculando el valor restante = 9 - 2 = 7 
            if(map[residue]){ // ahora comprobaremos si hay algún índice 7 presente. 
                const index = map[residue]; // desde aquí obtendré el índice para no. 7
                if(index == i) continue; // de ser igual el indice saltamos a la siguiente iteracción
                return [i, index]; // devolvemos la matriz con sus índices.
            }
        }
        return [];
    };

- Complejidad de tiempo: BigO(n) Recorrimos la lista que contiene n elementos solo una vez. Cada búsqueda en la tabla cuesta solo O(1) tiempo
- Complejidad del espacio: BigO(n) El espacio adicional requerido depende de la cantidad de elementos almacenados en la tabla map, que almacena como máximo n elementos


## Resultado:

| Tiempo de ejecución   | Memoria    |
|-----------------------|:-----------|
| 98 ms                 | 42.6 MB    |


## Con fuerza bruta es una solución muy ineficiente, ya que se debe recorrer la lista 2 veces.

    const twoSum = (nums, target) => {
        // este es el primer bucle
        for(let i = 0; i < nums.length; i++){
            // este es nuestro segundo buble y ayuda a proporcionar un valor por delante del valor anterior.
            for(let j = i + 1; j < nums.length; j++){
                // vamos a comparar el valor del segundo buble (j)
                // si este es igual a la resta del target menos el valor del primer buble (i)
                // entonces devolvemos los indices
                if(nums[j] == target - nums[i]){
                    return [i, j];
                }
            }
        }
        // si no puede obtener devolera una matriz vacia
        return [];
    };

- Complejidad de tiempo: BigO(n^2) Para cada elemento, intentamos encontrar su complemento recorriendo el resto de la matriz, lo que lleva O(n) tiempo. Por lo tanto, la complejidad del tiempo es O(n^2)
- Complejidad del espacio: BigO(1) El espacio requerido no depende del tamaño de la matriz de entrada, por lo que solo se usa espacio constante

<br>


## Resultado:

| Tiempo de ejecución   | Memoria    |
|-----------------------|:-----------|
| 928 ms                | 48.3 MB    |