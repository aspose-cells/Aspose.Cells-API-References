---
title: characters metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 30
url: /sv/python-net/aspose.cells/cell/characters/
is_root: false
---
##  characters(start_index, length) {#int-int}
Returnerar ett teckenobjekt som representerar ett intervall på characters inom celltexten.


###  Returnerar

Tecken objekt.


```python
def characters(self, start_index, length):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| start_index | int | Indexet för början av karaktären.|
| length | int | Antal tecken.|
###  Anmärkningar

Denna metod fungerar bara på cell med strängvärde.
###  Exempel


```python
from aspose.cells import Workbook
from aspose.pydrawing import Color

excel = Workbook()
cells = excel.worksheets[0].cells
cells.get("A1").put_value("Helloworld")
cells.get("A1").characters(5, 5).font.is_bold = True
cells.get("A1").characters(5, 5).font.color = Color.blue

```



###  Se även
* modul [aspose.cells](../../)
* klass [Cell](/cells/sv/python-net/aspose.cells/cell)
