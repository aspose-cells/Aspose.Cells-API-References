---
title: process_cell metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 20
url: /sv/python-net/aspose.cells/lightcellsdatahandler/process_cell/
is_root: false
---
##  process_cell(cell) {#Cell}
Börjar bearbeta en cell.


###  Returnerar

om denna cell behöver förvaras i cellmodell av aktuellt ark.
Vanligtvis bör det vara falskt så att alla celler inte kommer att lagras i minnet efter att ha bearbetats och sedan sparas minnet.
För något speciellt ändamål som att användaren behöver komma åt vissa celler senare efter att hela arbetsboken har bearbetats,
användaren kan få den här metoden att returnera sann för att behålla dessa speciella celler i Cells-modellen och komma åt dem senare med API:er som Cells[rad, kolumn].
Men att behålla celldata i Cells-modellen kräver mer minne och om alla celler behålls läser du mallfilen
i LightCells-läge blir det samma som att läsa det på vanligt sätt.


```python
def process_cell(self, cell):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| cell | [Cell](/cells/sv/python-net/aspose.cells/cell) | Cell objekt som bearbetas för närvarande|
###  Anmärkningar

Den kommer att anropas efter att en cells data har lästs.


###  Se även

* modul [aspose.cells](../../)
* klass [LightCellsDataHandler](/cells/sv/python-net/aspose.cells/lightcellsdatahandler)
