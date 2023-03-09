---
title: get_enumerator metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 40
url: /sv/python-net/aspose.cells/unionrange/get_enumerator/
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
bör inte ändras (som operationer som kommer att göra att nya Cell/Row instansieras eller befintliga Cell/Row tas bort).
Annars kanske uppräknaren inte kan gå igenom alla celler korrekt (vissa element kan korsas upprepade gånger eller hoppas över).


###  Se även
* modul [aspose.cells](../../)
* klass [UnionRange](/cells/sv/python-net/aspose.cells/unionrange)
