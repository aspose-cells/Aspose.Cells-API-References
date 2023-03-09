---
title: start_sheet metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 70
url: /sv/python-net/aspose.cells/lightcellsdataprovider/start_sheet/
is_root: false
---
##  start_sheet(sheet_index) {#int}
Börjar spara ett kalkylblad.


###  Returnerar

sant om denna leverantör kommer att tillhandahålla data för det givna bladet; falskt om det givna bladet ska använda sin normala datamodell (Cells).


```python
def start_sheet(self, sheet_index):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| sheet_index | int | index för aktuellt ark som ska sparas.|
###  Anmärkningar

Det kommer att anropas i början av att spara ett kalkylblad när du sparar en arbetsbok.
 Om leverantören behöver hänvisa till*`sheetIndex`* senare
i metoden startRow(Row) eller startCell(Cell),
 det vill säga om processen behöver veta vilket kalkylblad som bearbetas,
 genomförandet bör behålla*`sheetIndex`* värde här.


###  Se även
* modul [aspose.cells](../../)
* klass [LightCellsDataProvider](/cells/sv/python-net/aspose.cells/lightcellsdataprovider)
