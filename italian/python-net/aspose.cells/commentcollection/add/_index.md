---
title: metodo add
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 20
url: /it/python-net/aspose.cells/commentcollection/add/
is_root: false
---
##  add(cell_name) {#str}
Aggiunge un commento alla raccolta.


###  ritorna

[Comment](/cells/it/python-net/aspose.cells/comment) indice oggetto.


```python
def add(self, cell_name):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| cell_name | str | Cell nome.|

###  Esempio

```python

commentIndex2 = comments.add("B2")
comment2 = comments[commentIndex2]
comment2.note = "Second note."
comment2.font.name = "Times New Roman"

```


##  add(row, column) {#int-int}
Aggiunge un commento alla raccolta.


###  ritorna

[Comment](/cells/it/python-net/aspose.cells/comment) indice oggetto.


```python
def add(self, row, column):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| row | int | Cell indice riga.|
| column | int | Cell indice colonna.|

###  Esempio

```python

commentIndex1 = comments.add(0, 0)
comment1 = comments[commentIndex1]
comment1.note = "First note."
comment1.font.name = "Times New Roman"

```



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Comment](/cells/it/python-net/aspose.cells/comment)
* classe [CommentCollection](/cells/it/python-net/aspose.cells/commentcollection)
