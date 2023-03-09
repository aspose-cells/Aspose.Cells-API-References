---
title: get_enumerator metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 90
url: /sv/python-net/aspose.cells/range/get_enumerator/
is_root: false
---
##  get_enumerator() {#}
Hämtar enumeratorn för celler i detta intervall.


###  Returnerar

Celluppräkningen


```python
def get_enumerator(self):
    ...
```


###  Anmärkningar

När man korsar element av den returnerade Enumeratorn, samlas cellerna
bör inte ändras (som operationer som gör att nya Cell/Row instansieras eller befintliga Cell/Row tas bort).
Annars kanske uppräknaren inte kan gå igenom alla celler korrekt (vissa element kan korsas upprepade gånger eller hoppas över).
###  Exempel

```python
from aspose.cells import Workbook

workbook = Workbook("template.xlsx")
cells = workbook.worksheets[0].cells
en = cells.create_range("B2:C3").get_enumerator()
for cell in en:
    print(cell.name + ": "  + str(cell.value))

```



###  Se även
* modul [aspose.cells](../../)
* klass [Range](/cells/sv/python-net/aspose.cells/range)
