---
title: add_key método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells/datasorter/add_key/
is_root: false
---
##  add_key(key, order) {#int-SortOrder}
Agrega índice de columna ordenada y orden de clasificación.



```python
def add_key(self, key, order):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| key | int | El índice de la columna ordenada (posición absoluta, la columna A es 0, B es 1, ...)|
| order | [SortOrder](/cells/es/python-net/aspose.cells/sortorder) | el orden de clasificación|


##  add_key(key, order, custom_list) {#int-SortOrder-str}
Agrega índice de columna ordenado y orden de clasificación con lista de clasificación personalizada.



```python
def add_key(self, key, order, custom_list):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| key | int | El índice de la columna ordenada (posición absoluta, la columna A es 0, B es 1, ...)|
| order | [SortOrder](/cells/es/python-net/aspose.cells/sortorder) | El orden de clasificación.|
| custom_list | str | La lista de clasificación personalizada.|


##  add_key(key, order, custom_list) {#int-SortOrder-list}
Agrega índice de columna ordenado y orden de clasificación con lista de clasificación personalizada.



```python
def add_key(self, key, order, custom_list):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| key | int | El índice de la columna ordenada (posición absoluta, la columna A es 0, B es 1, ...)|
| order | [SortOrder](/cells/es/python-net/aspose.cells/sortorder) | El orden de clasificación.|
| custom_list | list | La lista de clasificación personalizada.|


##  add_key(key, type, order, custom_list) {#int-SortOnType-SortOrder-any}
Agrega índice de columna ordenado y orden de clasificación con lista de clasificación personalizada.



```python
def add_key(self, key, type, order, custom_list):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| key | int | El índice de la columna ordenada (posición absoluta, la columna A es 0, B es 1, ...)|
| type | [SortOnType](/cells/es/python-net/aspose.cells/sortontype) | El tipo de valor ordenado.|
| order | [SortOrder](/cells/es/python-net/aspose.cells/sortorder) | El orden de clasificación.|
| custom_list | any | La lista de clasificación personalizada.|
###  Observaciones

Si el tipo es SortOnType.CellColor o SortOnType.FontColor, la lista personalizada es Color.


###  Ver también

* módulo [aspose.cells](../../)
* clase [DataSorter](/cells/es/python-net/aspose.cells/datasorter)
