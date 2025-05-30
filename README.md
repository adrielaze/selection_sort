# selection_sort
Este repositório é para trabalho de algaritimo

# selection sort (ordenação por seleção)  ordenação ele percorre os numeros e ordena de nemor para o maior.
# vantagens ele e bom pra conjunto de dados pequenos.
# desvantagens para pratica em que a efeciencia e crucial ele n e bom.

lista = [10, 3, 7, 8, 2]

def selection_sort(lista):
    n = len(lista)
    for j in range(n - 1):
        minimo = j
        for i in range(j, n):
            if lista[i] < lista[minimo]:
                minimo = i
        if lista[j] > lista[minimo]:
            aux = lista[j]
            lista[j] = lista[minimo]
            lista[minimo] = aux
selection_sort(lista)
print(lista)
