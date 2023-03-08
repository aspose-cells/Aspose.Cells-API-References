---
title: start_row Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 60
url: /de/python-net/aspose.cells/lightcellsdataprovider/start_row/
is_root: false
---
##  start_row(row) {#Row}
Beginnt mit dem Speichern der Daten einer Zeile.



```python
def start_row(self, row):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| row | [Row](/cells/de/python-net/aspose.cells/row) | Zeilenobjekt für die Implementierung zum Füllen von Daten. Sein Zeilenindex ist der zurückgegebene Wert des letzten Aufrufs von [LightCellsDataProvider.next_row()](/cells/de/python-net/aspose.cells/lightcellsdataprovider/next_row).<br/>Wenn die Zeile im inneren Zellenmodell initialisiert wurde, wird das vorhandene Zeilenobjekt verwendet.<br/> Andernfalls wird ein temporäres Row-Objekt für die Implementierung verwendet, um Daten zu füllen.|
###  Bemerkungen

Es wird zu Beginn des Speicherns einer Zeile und ihrer Zellendaten aufgerufen.
Wenn die aktuelle Zeile einige benutzerdefinierte Eigenschaften wie Höhe, Stil usw. hat,
Die Implementierung sollte diese Eigenschaften hier auf das angegebene Row-Objekt setzen.


###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [LightCellsDataProvider](/cells/de/python-net/aspose.cells/lightcellsdataprovider)
