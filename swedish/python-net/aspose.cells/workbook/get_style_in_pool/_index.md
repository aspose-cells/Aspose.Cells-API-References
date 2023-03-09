---
title: get_style_in_pool metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 190
url: /sv/python-net/aspose.cells/workbook/get_style_in_pool/
is_root: false
---
##  get_style_in_pool(index) {#int}
Får stilen i stilpoolen.
Alla stilar i arbetsboken kommer att samlas i en pool.
Det finns bara ett enkelt referensindex i cellerna.


###  Returnerar

Stilen i poolen motsvarar givet index, kan vara null.


```python
def get_style_in_pool(self, index):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| index | int | Indexet.|
###  Anmärkningar

Om den returnerade stilen ändras, kommer stilen för alla celler (som hänvisar till denna stil) att ändras.


###  Se även

* modul [aspose.cells](../../)
* klass [Workbook](/cells/sv/python-net/aspose.cells/workbook)
