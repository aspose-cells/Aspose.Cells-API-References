---
title: start_sheet Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 70
url: /de/python-net/aspose.cells/lightcellsdataprovider/start_sheet/
is_root: false
---
##  start_sheet(sheet_index) {#int}
Beginnt mit dem Speichern eines Arbeitsblatts.


###  Kehrt zurück

wahr, wenn dieser Anbieter Daten für das angegebene Blatt bereitstellt; false, wenn das angegebene Blatt sein normales Datenmodell verwenden soll (Cells).


```python
def start_sheet(self, sheet_index):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| sheet_index | int | Index des aktuellen Blattes, das gespeichert werden soll.|
###  Bemerkungen

Es wird zu Beginn des Speicherns eines Arbeitsblatts während des Speicherns einer Arbeitsmappe aufgerufen.
 Wenn der Anbieter darauf verweisen muss*`sheetIndex`* später
in der Methode startRow(Row) oder startCell(Cell),
 das heißt, wenn der Prozess wissen muss, welches Arbeitsblatt verarbeitet wird,
 die Umsetzung sollte die beibehalten*`sheetIndex`* Wert hier.


###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [LightCellsDataProvider](/cells/de/python-net/aspose.cells/lightcellsdataprovider)
