---
title: HorizontalPageBreak classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 750
url: /fr/python-net/aspose.cells/horizontalpagebreak/
is_root: false
---
##  HorizontalPageBreak classe
Encapsule l'objet qui représente un saut de page horizontal.



Le type HorizontalPageBreak expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [start_column](/cells/fr/python-net/aspose.cells/horizontalpagebreak/start_column) | Obtient l'index de colonne de début de ce saut de page horizontal.|
| [end_column](/cells/fr/python-net/aspose.cells/horizontalpagebreak/end_column) | Obtient l'index de colonne de fin de ce saut de page horizontal.|
| [row](/cells/fr/python-net/aspose.cells/horizontalpagebreak/row) | Obtient l'index de ligne de base zéro.|



###  Exemple

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Add a page break at cell Y30
Index = worksheet.horizontal_page_breaks.add("Y30")
# get the newly added horizontal page break
hPageBreak = worksheet.horizontal_page_breaks[Index]

```

###  Voir également
* module [aspose.cells](..)
