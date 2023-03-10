---
title: page_scale propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 90
url: /fr/python-net/aspose.cells.rendering/sheetrender/page_scale/
is_root: false
---
##  page_scale propriété

Obtient l'échelle de page calculée de la feuille.
Renvoie l'échelle définie si [PageSetup.zoom](/cells/fr/python-net/aspose.cells/pagesetup#zoom) est défini. Sinon, renvoie l'échelle calculée selon [PageSetup.fit_to_pages_wide](/cells/fr/python-net/aspose.cells/pagesetup#fit_to_pages_wide) et [PageSetup.fit_to_pages_tall](/cells/fr/python-net/aspose.cells/pagesetup#fit_to_pages_tall).

###  Exemple

```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions, SheetRender

wb = Workbook("Book1.xlsx")
sheetRender = SheetRender(wb.worksheets[0], ImageOrPrintOptions())
# Gets calculated page scale of the sheet.
pageScale = sheetRender.page_scale

```
###  Définition:
```python
@property
def page_scale(self):
    ...
```

###  Voir également
* module [aspose.cells.rendering](../../)
* classe [SheetRender](/cells/fr/python-net/aspose.cells.rendering/sheetrender)
