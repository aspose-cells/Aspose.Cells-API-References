---
title: get_enumerator méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 90
url: /fr/python-net/aspose.cells/range/get_enumerator/
is_root: false
---
##  get_enumerator() {#}
Obtient l'énumérateur des cellules de cette plage.


###  Retour

L'énumérateur de cellules


```python
def get_enumerator(self):
    ...
```


###  Remarques

Lors de la traversée d'éléments par l'énumérateur renvoyé, la collection de cellules
ne doit pas être modifié (comme les opérations qui entraîneront l'instanciation d'un nouveau Cell/Row ou la suppression d'un Cell/Row existant).
Sinon, l'énumérateur peut ne pas être en mesure de parcourir correctement toutes les cellules (certains éléments peuvent être parcourus à plusieurs reprises ou ignorés).
###  Exemple

```python
from aspose.cells import Workbook

workbook = Workbook("template.xlsx")
cells = workbook.worksheets[0].cells
en = cells.create_range("B2:C3").get_enumerator()
for cell in en:
    print(cell.name + ": "  + str(cell.value))

```



###  Voir également
* module [aspose.cells](../../)
* classe [Range](/cells/fr/python-net/aspose.cells/range)
