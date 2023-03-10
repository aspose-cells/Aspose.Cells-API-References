---
title: add Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 20
url: /de/python-net/aspose.cells.timelines/timelinecollection/add/
is_root: false
---
##  add(pivot, dest_cell_name, base_field_name) {#aspose.cells.pivot.PivotTable-str-str}
Fügen Sie eine neue Zeitachse mit PivotTable als Datenquelle hinzu


###  Kehrt zurück

Der neue add Timeline-Index


```python
def add(self, pivot, dest_cell_name, base_field_name):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |PivotTable-Objekt|
| dest_cell_name | str | Der Zellenname in der oberen linken Ecke des Timeline-Bereichs.|
| base_field_name | str | Der Name von PivotField in PivotTable.BaseFields|

###  Beispiel

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, "i15", "date")

```


##  add(pivot, dest_cell_name, base_field_index) {#aspose.cells.pivot.PivotTable-str-int}
Fügen Sie eine neue Zeitachse mit PivotTable als Datenquelle hinzu


###  Kehrt zurück

Der neue add Timeline-Index


```python
def add(self, pivot, dest_cell_name, base_field_index):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |PivotTable-Objekt|
| dest_cell_name | str | Der Zellenname in der oberen linken Ecke des Timeline-Bereichs.|
| base_field_index | int | Der Index von PivotField in PivotTable.BaseFields|

###  Beispiel

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, "i5", 1)

```


##  add(pivot, dest_cell_name, base_field) {#aspose.cells.pivot.PivotTable-str-aspose.cells.pivot.PivotField}
Fügen Sie eine neue Zeitachse mit PivotTable als Datenquelle hinzu


###  Kehrt zurück

Der neue add Timeline-Index


```python
def add(self, pivot, dest_cell_name, base_field):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |PivotTable-Objekt|
| dest_cell_name | str | Der Zellenname in der oberen linken Ecke des Timeline-Bereichs.|
| base_field | aspose.cells.pivot.PivotField | Das PivotField in PivotTable.BaseFields|

###  Beispiel

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, "i10", pivot.base_fields[1])

```


##  add(pivot, row, column, base_field_name) {#aspose.cells.pivot.PivotTable-int-int-str}
Fügen Sie eine neue Zeitachse mit PivotTable als Datenquelle hinzu


###  Kehrt zurück

Der neue add Timeline-Index


```python
def add(self, pivot, row, column, base_field_name):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |PivotTable-Objekt|
| row | int | Zeilenindex der Zelle in der oberen linken Ecke des Timeline-Bereichs.|
| column | int | Spaltenindex der Zelle in der oberen linken Ecke des Timeline-Bereichs.|
| base_field_name | str | Der Name von PivotField in PivotTable.BaseFields|

###  Beispiel

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, 10, 5, "date")

```


##  add(pivot, row, column, base_field_index) {#aspose.cells.pivot.PivotTable-int-int-int}
Fügen Sie eine neue Zeitachse mit PivotTable als Datenquelle hinzu


###  Kehrt zurück

Der neue add Timeline-Index


```python
def add(self, pivot, row, column, base_field_index):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |PivotTable-Objekt|
| row | int | Zeilenindex der Zelle in der oberen linken Ecke des Timeline-Bereichs.|
| column | int | Spaltenindex der Zelle in der oberen linken Ecke des Timeline-Bereichs.|
| base_field_index | int | Der Index von PivotField in PivotTable.BaseFields|

###  Beispiel

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, 15, 5, 1)

```


##  add(pivot, row, column, base_field) {#aspose.cells.pivot.PivotTable-int-int-aspose.cells.pivot.PivotField}
Fügen Sie eine neue Zeitachse mit PivotTable als Datenquelle hinzu


###  Kehrt zurück

Der neue add Timeline-Index


```python
def add(self, pivot, row, column, base_field):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |PivotTable-Objekt|
| row | int | Zeilenindex der Zelle in der oberen linken Ecke des Timeline-Bereichs.|
| column | int | Spaltenindex der Zelle in der oberen linken Ecke des Timeline-Bereichs.|
| base_field | aspose.cells.pivot.PivotField | Das PivotField in PivotTable.BaseFields|

###  Beispiel

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, 20, 5, pivot.base_fields[1])

```



###  Siehe auch
* Modul [aspose.cells.timelines](../../)
* Klasse [TimelineCollection](/cells/de/python-net/aspose.cells.timelines/timelinecollection)
