---
title: process_cell Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 20
url: /de/python-net/aspose.cells/lightcellsdatahandler/process_cell/
is_root: false
---
##  process_cell(cell) {#Cell}
Beginnt mit der Verarbeitung einer Zelle.


###  Kehrt zurück

ob diese Zelle im Zellenmodell des aktuellen Blattes gehalten werden muss.
Im Allgemeinen sollte es falsch sein, damit nicht alle Zellen nach der Verarbeitung im Speicher bleiben und dann Speicher gespeichert wird.
Für einige spezielle Zwecke, z. B. wenn der Benutzer später auf einige Zellen zugreifen muss, nachdem die gesamte Arbeitsmappe verarbeitet wurde,
Der Benutzer kann dafür sorgen, dass diese Methode wahr zurückgibt, um diese speziellen Zellen im Cells-Modell zu behalten und später über APIs wie Cells [Zeile, Spalte] darauf zuzugreifen.
Das Aufbewahren von Zellendaten im Modell Cells erfordert jedoch mehr Speicher, und wenn alle Zellen beibehalten werden, muss die Vorlagendatei gelesen werden
im LightCells-Modus wird dasselbe wie beim Lesen auf normale Weise.


```python
def process_cell(self, cell):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| cell | [Cell](/cells/de/python-net/aspose.cells/cell) | Cell Objekt, das gerade bearbeitet wird|
###  Bemerkungen

Es wird aufgerufen, nachdem die Daten einer Zelle gelesen wurden.


###  Siehe auch

* Modul [aspose.cells](../../)
* Klasse [LightCellsDataHandler](/cells/de/python-net/aspose.cells/lightcellsdatahandler)
