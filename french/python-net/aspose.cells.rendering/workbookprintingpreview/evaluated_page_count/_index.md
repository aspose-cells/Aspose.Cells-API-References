---
title: evaluated_page_count propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 30
url: /fr/python-net/aspose.cells.rendering/workbookprintingpreview/evaluated_page_count/
is_root: false
---
##  evaluated_page_count propriété

Évaluer le nombre total de pages de ce classeur

###  Exemple

Le code suivant montre le moyen le plus rapide d'obtenir le nombre de pages d'un classeur.

```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions, WorkbookPrintingPreview

workbook = Workbook("Book1.xlsx")
workbookPrintingPreview = WorkbookPrintingPreview(workbook, ImageOrPrintOptions())
# fastest way to get page count especailly when there are massive data in workbook.
print(workbookPrintingPreview.evaluated_page_count)

```
###  Définition:
```python
@property
def evaluated_page_count(self):
    ...
```

###  Voir également
* module [aspose.cells.rendering](../../)
* classe [WorkbookPrintingPreview](/cells/fr/python-net/aspose.cells.rendering/workbookprintingpreview)
