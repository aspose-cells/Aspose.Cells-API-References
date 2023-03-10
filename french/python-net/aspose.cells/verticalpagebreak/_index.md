---
title: VerticalPageBreak classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1560
url: /fr/python-net/aspose.cells/verticalpagebreak/
is_root: false
---
##  VerticalPageBreak classe
Encapsule l'objet qui représente un saut de page vertical.



Le type VerticalPageBreak expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [start_row](/cells/fr/python-net/aspose.cells/verticalpagebreak/start_row) | Obtient l'index de ligne de début du saut de page vertical.|
| [end_row](/cells/fr/python-net/aspose.cells/verticalpagebreak/end_row) | Obtient l'index de fin de ligne du saut de page vertical.|
| [column](/cells/fr/python-net/aspose.cells/verticalpagebreak/column) | Obtient l'index de colonne du saut de page vertical.|



###  Exemple

```python
from aspose.cells import Workbook

excel = Workbook()
# Add a pagebreak at G5
excel.worksheets[0].horizontal_page_breaks.add("G5")
excel.worksheets[0].vertical_page_breaks.add("G5")

```

###  Voir également
* module [aspose.cells](..)
