---
title: characters méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 30
url: /fr/python-net/aspose.cells/cell/characters/
is_root: false
---
##  characters(start_index, length) {#int-int}
Renvoie un objet Characters qui représente une plage de characters dans le texte de la cellule.


###  Retour

Objet personnages.


```python
def characters(self, start_index, length):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| start_index | int | L'index du début du caractère.|
| length | int | Le nombre de caractères.|
###  Remarques

Cette méthode ne fonctionne que sur une cellule avec une valeur de chaîne.
###  Exemple


```python
from aspose.cells import Workbook
from aspose.pydrawing import Color

excel = Workbook()
cells = excel.worksheets[0].cells
cells.get("A1").put_value("Helloworld")
cells.get("A1").characters(5, 5).font.is_bold = True
cells.get("A1").characters(5, 5).font.color = Color.blue

```



###  Voir également
* module [aspose.cells](../../)
* classe [Cell](/cells/fr/python-net/aspose.cells/cell)
