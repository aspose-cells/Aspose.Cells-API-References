---
title: start_row metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 60
url: /sv/python-net/aspose.cells/lightcellsdataprovider/start_row/
is_root: false
---
##  start_row(row) {#Row}
Börjar spara data på en rad.



```python
def start_row(self, row):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| row | [Row](/cells/sv/python-net/aspose.cells/row) | Radobjekt för implementering för att fylla data. Dess radindex är det returnerade värdet av senaste samtalet [LightCellsDataProvider.next_row()](/cells/sv/python-net/aspose.cells/lightcellsdataprovider/next_row).<br/>Om raden har initierats i modellen med inre celler kommer det befintliga radobjektet att användas.<br/> Annars kommer ett temporärt radobjekt att användas för implementering för att fylla data.|
###  Anmärkningar

Den kommer att anropas i början av att spara en rad och dess celldata.
Om den aktuella raden har några anpassade egenskaper som höjd, stil, ... etc.,
implementering bör ställa in dessa egenskaper till ett givet radobjekt här.


###  Se även
* modul [aspose.cells](../../)
* klass [LightCellsDataProvider](/cells/sv/python-net/aspose.cells/lightcellsdataprovider)
