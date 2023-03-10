---
title: start_cell metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 40
url: /sv/python-net/aspose.cells/lightcellsdatahandler/start_cell/
is_root: false
---
##  start_cell(column_index) {#int}
Förbereder bearbetning av en cell.


###  Returnerar

om denna cell behöver bearbetas. false för att ignorera cellen och kontrollera nästa tills du når slutet av celldata för den aktuella raden


```python
def start_cell(self, column_index):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| column_index | int | kolumnindex för cellen som ska bearbetas|
###  Anmärkningar

Den kommer att anropas när du når en befintlig cell i den aktuella raden. Den aktuella raden är raden för det senaste samtalet på [LightCellsDataHandler.process_row(row)](/cells/sv/python-net/aspose.cells/lightcellsdatahandler/process_row).


###  Se även

* modul [aspose.cells](../../)
* klass [LightCellsDataHandler](/cells/sv/python-net/aspose.cells/lightcellsdatahandler)
