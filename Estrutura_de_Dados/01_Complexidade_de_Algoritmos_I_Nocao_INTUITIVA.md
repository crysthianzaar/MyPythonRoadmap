- Complexidade → Serve para analisar a eficiencia de um programa
- PROGRAMA E ALGORITMO NÃO SÃO A MESMA COISA
- Quando se fala em complexidade de algoritmos, primeiro se foca na questão do tempo de processamento e não no espaço.

```python
#Exemplo para entender o conceito de complexidade

def inverter_lista(lista):
	tamanho = len(lista)
	limite = tamanho//2
	for i in range(limite)
		aux = lista[i]
		lista[i] = lista[tamanho-i]
		lista [tamanho-i] = aux

#Complexidade de Espaço (Memória): 4 + N ( 4 variáveis + N elementos da lista)
#Para calcular processamento, tomamos como base operações elementares:
#Complexidade de Tempo (Processamento): 2 + 3*(N/2) (tamanho,limite + linhas do for)

def inverter_lista2(lista):
	nova_lista  = []
	tamanho = len(lista)
	for i in range(tamanho):
		nova_lista.append(lista[tamanho-1]
	return nova_lista

#Complexidade de Tempo : 2+N
#Complexidade de Espaço: 3+ 2*N
```

- Complexidade é uma medida da quantidade de recursos que são demandados por um algoritmo. Podendo ser complexidade de tempo ou de espaço
- Para calcular complexidade fazemos contas pouco detalhadas