- 
    
    ```python
    def inverter_lista(lista):
    	tamanho = len(lista)
    	limite = tamanho//2
    	for i in range(limite)
    		aux = lista[i]
    		lista[i] = lista[tamanho-i]
    		lista [tamanho-i] = aux
    
    #Complexidade de Tempo: 2 + 4*(N/2) -> 2 + 2*N
    ```
    
    - Ou seja, o 2*N é o termo dominante pois ele que vai ditar a qtd de recursos.
    - O(n) → significa que o termo dominante está relacionado ao N.
    
    ```python
    def tem_duplicados(lista):
    	for i in range(len(lista)-1):
    		for j in range(i+1,len(lista)):
    			if lista[i] == lista[j]:
    				return True
    	return False
    
    #Complexidade de tempo: N*(N-1)/2 -> (N^2 - N) /2 -> O(n^2)
    ```
    
    - Complexidade é uma medida da quantidade de recursos que são demandados por um algoritmo. Podendo ser complexidade de tempo ou de espaço
    - O que mais importa a cerca da complexidade de algoritmos é como ela cresce com o tamanho da entrada
    - Expressamos a complexidade de algoritmos utilizando a notação do O grande, focando no termo dominante
    - Sempre analisar a complexidade do pior cenário (maior número de operações)