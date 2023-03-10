---
title: index_of método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 40
url: /es/python-net/aspose.cells.properties/documentpropertycollection/index_of/
is_root: false
---
##  index_of(name) {#str}
Obtiene el índice de una propiedad por nombre.


###  Devoluciones

El índice de base cero. Valor negativo si no se encuentra.


```python
def index_of(self, name):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| name | str | El nombre de la propiedad que no distingue entre mayúsculas y minúsculas.|


##  index_of(item, index) {#DocumentProperty-int}
Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el índice especificado hasta el último elemento.


###  Devoluciones

El índice de base cero de la primera aparición de valor dentro del rango de elementos en la lista de matriz que se extiende desde startIndex hasta el último elemento, si se encuentra; de lo contrario, -1.


```python
def index_of(self, item, index):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| item | [DocumentProperty](/cells/es/python-net/aspose.cells.properties/documentproperty) | El objeto a ubicar en la lista de matrices. El valor puede ser nulo.|
| index | int | El índice inicial de base cero de la búsqueda. 0 (cero) es válido en una lista vacía.|


##  index_of(item, index, count) {#DocumentProperty-int-int}
Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de matriz que comienza en el índice especificado y contiene el número especificado de elementos.


###  Devoluciones

El índice de base cero de la primera aparición de valor dentro del rango de elementos en la lista de matriz que comienza en startIndex y contiene el número de elementos, si se encuentra; de lo contrario, -1.


```python
def index_of(self, item, index, count):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| item | [DocumentProperty](/cells/es/python-net/aspose.cells.properties/documentproperty) | El objeto a ubicar en la lista de matrices. El valor puede ser nulo.|
| index | int | El índice inicial de base cero de la búsqueda. 0 (cero) es válido en una lista vacía.|
| count | int | El número de elementos en la sección a buscar.|



###  Ver también
* módulo [aspose.cells.properties](../../)
* clase [DocumentPropertyCollection](/cells/es/python-net/aspose.cells.properties/documentpropertycollection)
