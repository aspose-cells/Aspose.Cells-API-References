---
title: add método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells/commentcollection/add/
is_root: false
---
##  add(cell_name) {#str}
Añade un comentario a la colección.


###  Devoluciones

[Comment](/cells/es/python-net/aspose.cells/comment) índice de objetos.


```python
def add(self, cell_name):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| cell_name | str | Cell nombre.|

###  Ejemplos

```python

commentIndex2 = comments.add("B2")
comment2 = comments[commentIndex2]
comment2.note = "Second note."
comment2.font.name = "Times New Roman"

```


##  add(row, column) {#int-int}
Añade un comentario a la colección.


###  Devoluciones

[Comment](/cells/es/python-net/aspose.cells/comment) índice de objetos.


```python
def add(self, row, column):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| row | int | Cell índice de fila.|
| column | int | Cell índice de columna.|

###  Ejemplos

```python

commentIndex1 = comments.add(0, 0)
comment1 = comments[commentIndex1]
comment1.note = "First note."
comment1.font.name = "Times New Roman"

```



###  Ver también
* módulo [aspose.cells](../../)
* clase [Comment](/cells/es/python-net/aspose.cells/comment)
* clase [CommentCollection](/cells/es/python-net/aspose.cells/commentcollection)
