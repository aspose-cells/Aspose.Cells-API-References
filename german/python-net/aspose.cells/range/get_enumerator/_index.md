---
title: get_enumerator Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 90
url: /de/python-net/aspose.cells/range/get_enumerator/
is_root: false
---
##  get_enumerator() {#}
Ruft den Enumerator für Zellen in diesem Bereich ab.


###  Kehrt zurück

Der Zellenzähler


```python
def get_enumerator(self):
    ...
```


###  Bemerkungen

Beim Durchlaufen von Elementen durch den zurückgegebenen Enumerator, die Zellensammlung
sollten nicht geändert werden (z. B. Operationen, die dazu führen, dass neue Cell/Row instanziiert oder vorhandene Cell/Row gelöscht werden).
Andernfalls ist der Enumerator möglicherweise nicht in der Lage, alle Zellen korrekt zu durchlaufen (einige Elemente werden möglicherweise wiederholt durchlaufen oder übersprungen).
###  Beispiel

```python
from aspose.cells import Workbook

workbook = Workbook("template.xlsx")
cells = workbook.worksheets[0].cells
en = cells.create_range("B2:C3").get_enumerator()
for cell in en:
    print(cell.name + ": "  + str(cell.value))

```



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Range](/cells/de/python-net/aspose.cells/range)
