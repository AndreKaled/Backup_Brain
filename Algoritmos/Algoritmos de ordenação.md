# O que são algoritmos de ordenação?
Algoritmos de ordenação são métodos computacionais que organizam dados em uma sequência específica, como crescente ou decrescente, seguindo critérios definidos. Eles são amplamente utilizados para facilitar a busca eficiente de informações e otimizar operações que dependem da ordem dos dados.

---
# Exemplos em Python
## Bubble Sort
Um dos mais simples, porém ineficientes para grandes conjuntos de dados. Compara e troca elementos adjacentes repetidamente até que a lista esteja ordenada.
```python
def bubble_sort(lista):
   lst = lista.copy()
   desordenado = False
   for i in range(len(lst)):
      desordenado = False
      for j in range(len(lst)-i-1):
         if lst[j] > lst[j+1]:	#faz a troca, se for maior
            aux = lst[j+1]
            lst[j+1] = lst[j]
            lst[j] = aux
            desordenado = True
      if not desordenado:	#retorna a lista se já estiver ordenada
         return lst
	
print("Bubble:    ", bubble_sort(l)
```

## Selection Sort
Encontra o menor (ou maior) elemento e o coloca na posição correta, repetindo o processo para o restante da lista. É também ineficiente para grandes conjuntos.
```python
def selection_sort(lista):
   lst = lista.copy()
   for i in range(len(lst)):
		#selecionando indice menor prioritário
      menor = i
      for j in range(i+1,len(lst)):
         if lst[menor] > lst[j]:	#verificando se realmente é o menor, senão, troca-o
            menor = j
      if menor != i:	#se for diferente, faz a troca dos elementos
         aux = lst[i]
         lst[i] = lst[menor]
         lst[menor] = aux
   return lst
		
print("Selection: ", selection_sort(l))	
```

## Insertion Sort
Constrói a ordenação final um elemento por vez, inserindo cada novo elemento na posição correta em uma lista previamente ordenada. Funciona bem para listas pequenas ou quase ordenadas.
```python
def insertion_sort(lista):
   lst = lista.copy()
   for i in range(1,len(lst)):
      valor = lst[i]
      j = i-1	#acessando a esquerda da lista
      while j >= 0 and lst[j] > valor:
         lst[j+1] = lst[j]	#trocando posições até que ache o menor valor
         j -= 1
      lst[j+1] = valor	#inserindo na posição o valor menor, ordenado
   return lst

print("Insertion: ", insertion_sort(l))
```

## Merge Sort
Divide a lista em sublistas menores, ordena cada sublista e depois as combina (merge) de volta em uma lista ordenada. Utiliza a abordagem de divisão e conquista e tem complexidade de tempo O(n log n).
## Quick Sort
Seleciona um elemento como pivô e particiona a lista em dois subgrupos: um com elementos menores que o pivô e outro com elementos maiores. Ordena os subgrupos recursivamente. Também usa divisão e conquista e é eficiente para grandes conjuntos, com complexidade média de O(n log n).
## Herp Sort
Constrói uma estrutura de dados em forma de heap a partir da lista e extrai o maior (ou menor) elemento repetidamente para formar a lista ordenada. Tem complexidade de tempo O(n log n).

---
# Eficácia aplicada

| Algoritmo | Melhor caso | Caso médio | Pior caso | Uso de memória auxiliar |
| --------- | ----------- | ---------- | --------- | ----------------------- |
|           |             |            |           |                         |
|           |             |            |           |                         |


---
#Bubble #Selection #Insertion #Merge #Quick #Ordenação #Algoritmo