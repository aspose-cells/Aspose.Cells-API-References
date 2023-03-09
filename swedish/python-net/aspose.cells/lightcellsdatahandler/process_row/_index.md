---
title: process_row metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 30
url: /sv/python-net/aspose.cells/lightcellsdatahandler/process_row/
is_root: false
---
##  process_row(row) {#Row}
Börjar bearbeta en rad.


###  Returnerar

om den här radens celler behöver bearbetas. false för att ignorera alla celler i den här raden.


```python
def process_row(self, row):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| row | [Row](/cells/sv/python-net/aspose.cells/row) | Radobjekt som för närvarande bearbetas.|
###  Anmärkningar

Det kommer att kallas efter radens egenskaper som höjd, stil, ... etc. har lästs. Cellerna i den här raden har dock inte lästs ännu.


###  Se även

* modul [aspose.cells](../../)
* klass [LightCellsDataHandler](/cells/sv/python-net/aspose.cells/lightcellsdatahandler)
