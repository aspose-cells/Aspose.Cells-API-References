---
title: process_row Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 30
url: /de/python-net/aspose.cells/lightcellsdatahandler/process_row/
is_root: false
---
##  process_row(row) {#Row}
Beginnt mit der Verarbeitung einer Zeile.


###  Kehrt zurück

ob die Zellen dieser Zeile verarbeitet werden müssen. false, um alle Zellen in dieser Zeile zu ignorieren.


```python
def process_row(self, row):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| row | [Row](/cells/de/python-net/aspose.cells/row) | Zeilenobjekt, das gerade verarbeitet wird.|
###  Bemerkungen

Es wird nach den Eigenschaften der Zeile wie Höhe, Stil usw. aufgerufen. wurden gelesen. Zellen in dieser Zeile wurden jedoch noch nicht gelesen.


###  Siehe auch

* Modul [aspose.cells](../../)
* Klasse [LightCellsDataHandler](/cells/de/python-net/aspose.cells/lightcellsdatahandler)
