---
title: metodo get_enumerator
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 90
url: /it/python-net/aspose.cells/range/get_enumerator/
is_root: false
---
##  get_enumerator() {#}
Ottiene l'enumeratore per le celle in questo Range.


###  ritorna

L'enumeratore di celle


```python
def get_enumerator(self):
    ...
```


###  Osservazioni

Quando si attraversano gli elementi dall'enumeratore restituito, la raccolta di celle
non deve essere modificato (come le operazioni che provocheranno la creazione di un'istanza del nuovo Cell/Row o l'eliminazione di Cell/Row esistente).
In caso contrario, l'enumeratore potrebbe non essere in grado di attraversare correttamente tutte le celle (alcuni elementi potrebbero essere attraversati ripetutamente o ignorati).
###  Esempio

```python
from aspose.cells import Workbook

workbook = Workbook("template.xlsx")
cells = workbook.worksheets[0].cells
en = cells.create_range("B2:C3").get_enumerator()
for cell in en:
    print(cell.name + ": "  + str(cell.value))

```



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Range](/cells/it/python-net/aspose.cells/range)
