---
title: add Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 20
url: /de/python-net/aspose.cells.charts/chartcollection/add/
is_root: false
---
##  add(type, upper_left_row, upper_left_column, lower_right_row, lower_right_column) {#ChartType-int-int-int-int}
Fügt der Sammlung ein Diagramm hinzu.


###  Kehrt zurück

[Chart](/cells/de/python-net/aspose.cells.charts/chart) Objektindex.


```python
def add(self, type, upper_left_row, upper_left_column, lower_right_row, lower_right_column):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| type | [ChartType](/cells/de/python-net/aspose.cells.charts/charttype) | Diagramm Typ|
| upper_left_row | int | Zeilenindex oben links.|
| upper_left_column | int |Spaltenindex oben links.|
| lower_right_row | int | Zeilenindex unten rechts|
| lower_right_column | int | Spaltenindex unten rechts|


##  add(type, data_range, top_row, left_column, right_row, bottom_column) {#ChartType-str-int-int-int-int}
Fügt der Sammlung ein Diagramm hinzu.


###  Kehrt zurück

[Chart](/cells/de/python-net/aspose.cells.charts/chart) Objektindex.


```python
def add(self, type, data_range, top_row, left_column, right_row, bottom_column):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| type | [ChartType](/cells/de/python-net/aspose.cells.charts/charttype) | Diagramm Typ|
| data_range | str |Gibt den Datenbereich des Diagramms an|
| top_row | int | Zeilenindex oben links.|
| left_column | int |Spaltenindex oben links.|
| right_row | int | Zeilenindex unten rechts|
| bottom_column | int | Spaltenindex unten rechts|
###  Bemerkungen

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen,
Bitte verwenden Sie die Eigenschaft [ChartCollection.add(type, upper_left_row, upper_left_column, lower_right_row, lower_right_column)](/cells/de/python-net/aspose.cells.charts/chartcollection/add).
Diese Property wird 12 Monate später seit Mai 2022 entfernt.
Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

##  add(data, data_range, is_vertical, top_row, left_column, right_row, bottom_column) {#bytes-str-bool-int-int-int-int}
Fügt ein Diagramm mit voreingestellter Vorlage hinzu.


###  Kehrt zurück

[Chart](/cells/de/python-net/aspose.cells.charts/chart) Objektindex.


```python
def add(self, data, data_range, is_vertical, top_row, left_column, right_row, bottom_column):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| data | bytes | Die Daten der Diagrammvorlagendatei (.crtx).|
| data_range | str |Gibt den Datenbereich des Diagramms an|
| is_vertical | bool | Gibt an, ob die Reihe aus einem Bereich von Zellenwerten zeilen- oder spaltenweise dargestellt werden soll.|
| top_row | int | Zeilenindex oben links.|
| left_column | int |Spaltenindex oben links.|
| right_row | int | Zeilenindex unten rechts|
| bottom_column | int | Spaltenindex unten rechts|


##  add(type, data_range, is_vertical, top_row, left_column, right_row, bottom_column) {#ChartType-str-bool-int-int-int-int}
Fügt der Sammlung ein Diagramm hinzu.


###  Kehrt zurück

[Chart](/cells/de/python-net/aspose.cells.charts/chart) Objektindex.


```python
def add(self, type, data_range, is_vertical, top_row, left_column, right_row, bottom_column):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| type | [ChartType](/cells/de/python-net/aspose.cells.charts/charttype) | Diagramm Typ|
| data_range | str |Gibt den Datenbereich des Diagramms an|
| is_vertical | bool | Gibt an, ob die Reihe aus einem Bereich von Zellenwerten zeilen- oder spaltenweise dargestellt werden soll.|
| top_row | int | Zeilenindex oben links.|
| left_column | int |Spaltenindex oben links.|
| right_row | int | Zeilenindex unten rechts|
| bottom_column | int | Spaltenindex unten rechts|



###  Siehe auch
* Modul [aspose.cells.charts](../../)
* Klasse [Chart](/cells/de/python-net/aspose.cells.charts/chart)
* Klasse [ChartCollection](/cells/de/python-net/aspose.cells.charts/chartcollection)
