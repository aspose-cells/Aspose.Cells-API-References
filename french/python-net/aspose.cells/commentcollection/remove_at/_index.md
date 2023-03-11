---
title: remove_at méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 90
url: /fr/python-net/aspose.cells/commentcollection/remove_at/
is_root: false
---
##  remove_at(cell_name) {#str}
Supprime le commentaire de la cellule spécifique.



```python
def remove_at(self, cell_name):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| cell_name | str | Le nom de la cellule qui contient un commentaire.|

###  Exemple

```python

comments.remove_at("B2")

```


##  remove_at(row, column) {#int-int}
Supprime le commentaire de la cellule spécifique.



```python
def remove_at(self, row, column):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| row | int | L'index de ligne.|
| column | int | l'indice de colonne.|

###  Exemple

```python

comments.remove_at(1, 1)

```



###  Voir également
* module [aspose.cells](../../)
* classe [CommentCollection](/cells/fr/python-net/aspose.cells/commentcollection)
