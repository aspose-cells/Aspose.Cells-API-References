---
title: add méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 20
url: /fr/python-net/aspose.cells.drawing/textboxcollection/add/
is_root: false
---
##  add(upper_left_row, upper_left_column, height, width) {#int-int-int-int}
Ajoute une zone de texte à la collection.


###  Retour

[TextBox](/cells/fr/python-net/aspose.cells.drawing/textbox) indice d'objet.


```python
def add(self, upper_left_row, upper_left_column, height, width):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| upper_left_row | int | Index de ligne en haut à gauche.|
| upper_left_column | int |Index de la colonne en haut à gauche.|
| height | int | Hauteur de la zone de texte, en unité de pixel.|
| width | int | Largeur de la zone de texte, en unité de pixel.|

###  Exemple

```python

# add a TextBox
index2 = textBoxCollection.add(1, 1, 50, 100)

```



###  Voir également
* module [aspose.cells.drawing](../../)
* classe [TextBox](/cells/fr/python-net/aspose.cells.drawing/textbox)
* classe [TextBoxCollection](/cells/fr/python-net/aspose.cells.drawing/textboxcollection)
