---
title: start_cell Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 40
url: /de/python-net/aspose.cells/lightcellsdatahandler/start_cell/
is_root: false
---
##  start_cell(column_index) {#int}
Bereitet die Verarbeitung einer Zelle vor.


###  Kehrt zurück

ob diese Zelle verarbeitet werden muss false, um die Zelle zu ignorieren und die nächste zu prüfen, bis das Ende der Zellendaten der aktuellen Zeile erreicht ist


```python
def start_cell(self, column_index):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| column_index | int | Spaltenindex der zu verarbeitenden Zelle|
###  Bemerkungen

Es wird aufgerufen, wenn eine vorhandene Zelle in der aktuellen Zeile erreicht wird. Die aktuelle Zeile ist die Zeile des letzten Anrufs von [LightCellsDataHandler.process_row(row)](/cells/de/python-net/aspose.cells/lightcellsdatahandler/process_row).


###  Siehe auch

* Modul [aspose.cells](../../)
* Klasse [LightCellsDataHandler](/cells/de/python-net/aspose.cells/lightcellsdatahandler)
