---
title: page_scale Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 90
url: /de/python-net/aspose.cells.rendering/sheetrender/page_scale/
is_root: false
---
##  page_scale Eigentum

Ruft den berechneten Seitenmaßstab des Blatts ab.
Gibt die eingestellte Skala zurück, wenn [PageSetup.zoom](/cells/de/python-net/aspose.cells/pagesetup#zoom) eingestellt ist.

###  Beispiele

```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions, SheetRender

wb = Workbook("Book1.xlsx")
sheetRender = SheetRender(wb.worksheets[0], ImageOrPrintOptions())
# Gets calculated page scale of the sheet.
pageScale = sheetRender.page_scale

```
###  Definition:
```python
@property
def page_scale(self):
    ...
```

###  Siehe auch
* Modul [aspose.cells.rendering](../../)
* Klasse [SheetRender](/cells/de/python-net/aspose.cells.rendering/sheetrender)
