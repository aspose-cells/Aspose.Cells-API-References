---
title: get_threaded_comments méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 60
url: /fr/python-net/aspose.cells/commentcollection/get_threaded_comments/
is_root: false
---
##  get_threaded_comments(cell_name) {#str}
Obtient les commentaires thématiques par nom de cellule.


###  Retour




```python
def get_threaded_comments(self, cell_name):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| cell_name | str | Le nom de la cellule.|

###  Exemple

```python

threadedComments2 = comments.get_threaded_comments("B2")
for i in range(len(threadedComments2)):
    tc = threadedComments2[i]
    note = tc.notes

```


##  get_threaded_comments(row, column) {#int-int}
Obtient les commentaires thématiques par index de ligne et de colonne.


###  Retour




```python
def get_threaded_comments(self, row, column):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| row | int | L'index de ligne.|
| column | int | L'indice de colonne.|

###  Exemple

```python

threadedComments1 = comments.get_threaded_comments(1, 1)
for i in range(len(threadedComments1)):
    tc = threadedComments1[i]
    note = tc.notes

```



###  Voir également
* module [aspose.cells](../../)
* classe [CommentCollection](/cells/fr/python-net/aspose.cells/commentcollection)
