---
title: add méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 20
url: /fr/python-net/aspose.cells/commentcollection/add/
is_root: false
---
##  add(cell_name) {#str}
Ajoute un commentaire à la collection.


###  Retour

[Comment](/cells/fr/python-net/aspose.cells/comment) indice d'objet.


```python
def add(self, cell_name):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| cell_name | str | Cell nom.|

###  Exemple

```python

commentIndex2 = comments.add("B2")
comment2 = comments[commentIndex2]
comment2.note = "Second note."
comment2.font.name = "Times New Roman"

```


##  add(row, column) {#int-int}
Ajoute un commentaire à la collection.


###  Retour

[Comment](/cells/fr/python-net/aspose.cells/comment) indice d'objet.


```python
def add(self, row, column):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| row | int | Cell index de ligne.|
| column | int | Cell index de colonne.|

###  Exemple

```python

commentIndex1 = comments.add(0, 0)
comment1 = comments[commentIndex1]
comment1.note = "First note."
comment1.font.name = "Times New Roman"

```



###  Voir également
* module [aspose.cells](../../)
* classe [Comment](/cells/fr/python-net/aspose.cells/comment)
* classe [CommentCollection](/cells/fr/python-net/aspose.cells/commentcollection)
