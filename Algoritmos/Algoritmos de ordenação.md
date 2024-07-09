## Bubble sort


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

## Selection sort


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

## Insertion sort


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

## Merge sort
# Quick sort