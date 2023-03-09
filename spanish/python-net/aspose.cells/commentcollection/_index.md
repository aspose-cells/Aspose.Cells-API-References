---
title: CommentCollection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 290
url: /es/python-net/aspose.cells/commentcollection/
is_root: false
---
##  CommentCollection clase
Encapsula una colección de [Comment](/cells/es/python-net/aspose.cells/comment) objetos.



El tipo CommentCollection expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [capacity](/cells/es/python-net/aspose.cells/commentcollection/capacity) | Obtiene o establece el número de elementos que puede contener la lista de matrices.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [add_threaded_comment(row, column, text, author)](/cells/es/python-net/aspose.cells/commentcollection/add_threaded_comment/#int-int-str-ThreadedCommentAuthor) | Agrega un comentario encadenado.|
| [add_threaded_comment(cell_name, text, author)](/cells/es/python-net/aspose.cells/commentcollection/add_threaded_comment/#str-str-ThreadedCommentAuthor) | Agrega un comentario encadenado.|
| [get_threaded_comments(row, column)](/cells/es/python-net/aspose.cells/commentcollection/get_threaded_comments/#int-int) | Obtiene los comentarios encadenados por índice de fila y columna.|
| [get_threaded_comments(cell_name)](/cells/es/python-net/aspose.cells/commentcollection/get_threaded_comments/#str) | Obtiene los comentarios encadenados por nombre de celda.|
| [add(row, column)](/cells/es/python-net/aspose.cells/commentcollection/add/#int-int) | Añade un comentario a la colección.|
| [add(cell_name)](/cells/es/python-net/aspose.cells/commentcollection/add/#str) | Añade un comentario a la colección.|
| [remove_at(cell_name)](/cells/es/python-net/aspose.cells/commentcollection/remove_at/#str) | Elimina el comentario de la celda específica.|
| [remove_at(row, column)](/cells/es/python-net/aspose.cells/commentcollection/remove_at/#int-int) | Elimina el comentario de la celda específica.|
| [copy_to(array)](/cells/es/python-net/aspose.cells/commentcollection/copy_to/#list) | Copia toda la lista de matrices en una lista de matrices unidimensional compatible, comenzando por el principio de la lista de matrices de destino.|
| [copy_to(index, array, array_index, count)](/cells/es/python-net/aspose.cells/commentcollection/copy_to/#int-list-int-int) | Copia un rango de elementos de la lista de arreglos a una lista de arreglos unidimensional compatible, comenzando en el índice especificado de la lista de arreglos de destino.|
| [index_of(item, index)](/cells/es/python-net/aspose.cells/commentcollection/index_of/#Comment-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el índice especificado hasta el último elemento.|
| [index_of(item, index, count)](/cells/es/python-net/aspose.cells/commentcollection/index_of/#Comment-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de matriz que comienza en el índice especificado y contiene el número especificado de elementos.|
| [last_index_of(item)](/cells/es/python-net/aspose.cells/commentcollection/last_index_of/#Comment) | Busca el objeto especificado y devuelve el índice de base cero de la última aparición en toda la lista de matrices.|
| [last_index_of(item, index)](/cells/es/python-net/aspose.cells/commentcollection/last_index_of/#Comment-int) |Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el primer elemento hasta el índice especificado.|
| [last_index_of(item, index, count)](/cells/es/python-net/aspose.cells/commentcollection/last_index_of/#Comment-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de matriz que contiene el número especificado de elementos y termina en el índice especificado.|
| [binary_search(item)](/cells/es/python-net/aspose.cells/commentcollection/binary_search/#Comment) | Busca un elemento en toda la lista de matrices ordenadas mediante el comparador predeterminado y devuelve el índice de base cero del elemento.|



###  Ejemplo

```python
from aspose.cells import Workbook

workbook = Workbook()
comments = workbook.worksheets[0].comments

```

###  Ver también
* módulo [aspose.cells](..)
* clase [Comment](/cells/es/python-net/aspose.cells/comment)
