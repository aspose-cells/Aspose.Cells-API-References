---
title: add metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 20
url: /sv/python-net/aspose.cells.slicers/slicercollection/add/
is_root: false
---
##  add(pivot, dest_cell_name, base_field_name) {#aspose.cells.pivot.PivotTable-str-str}
Lägg till en ny Slicer med pivottabell som datakälla


###  Returnerar

Det nya add Slicer-index


```python
def add(self, pivot, dest_cell_name, base_field_name):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Pivottabellobjekt|
| dest_cell_name | str | Cellen i det övre vänstra hörnet av Slicer-intervallet.|
| base_field_name | str | Namnet på PivotField i PivotTable.BaseFields|

###  Exempel

```python

slicers.add(pivot, "E3", "fruit")

```


##  add(pivot, dest_cell_name, base_field_index) {#aspose.cells.pivot.PivotTable-str-int}
Lägg till en ny Slicer med pivottabell som datakälla


###  Returnerar

Det nya add Slicer-index


```python
def add(self, pivot, dest_cell_name, base_field_index):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Pivottabellobjekt|
| dest_cell_name | str | Cellen i det övre vänstra hörnet av Slicer-intervallet.|
| base_field_index | int | Indexet för PivotField i PivotTable.BaseFields|

###  Exempel

```python

slicers.add(pivot, "E20", 0)

```


##  add(pivot, dest_cell_name, base_field) {#aspose.cells.pivot.PivotTable-str-aspose.cells.pivot.PivotField}
Lägg till en ny Slicer med pivottabell som datakälla


###  Returnerar

Det nya add Slicer-index


```python
def add(self, pivot, dest_cell_name, base_field):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Pivottabellobjekt|
| dest_cell_name | str | Cellen i det övre vänstra hörnet av Slicer-intervallet.|
| base_field | aspose.cells.pivot.PivotField | Pivotfältet i PivotTable.BaseFields|

###  Exempel

```python

slicers.add(pivot, "I3", pivot.base_fields[0])

```


##  add(table, index, dest_cell_name) {#aspose.cells.tables.ListObject-int-str}
Lägg till en ny Slicer med ListObjet som datakälla


###  Returnerar

Det nya add Slicer-index


```python
def add(self, table, index, dest_cell_name):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| table | aspose.cells.tables.ListObject | ListObject-objekt|
| index | int | Indexet för ListColumn i ListObject.ListColumns|
| dest_cell_name | str | Cellen i det övre vänstra hörnet av Slicer-intervallet.|

###  Exempel

```python

slicers.add(table, 1, "E38")

```


##  add(table, list_column, dest_cell_name) {#aspose.cells.tables.ListObject-aspose.cells.tables.ListColumn-str}
Lägg till en ny Slicer med ListObjet som datakälla


###  Returnerar

Det nya add Slicer-index


```python
def add(self, table, list_column, dest_cell_name):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| table | aspose.cells.tables.ListObject | ListObject-objekt|
| list_column | aspose.cells.tables.ListColumn | Listkolumnen i ListObject.ListColumns|
| dest_cell_name | str | Cellen i det övre vänstra hörnet av Slicer-intervallet.|

###  Exempel

```python

slicers.add(table, table.list_columns[1], "I38")

```


##  add(pivot, row, column, base_field_name) {#aspose.cells.pivot.PivotTable-int-int-str}
Lägg till en ny Slicer med pivottabell som datakälla


###  Returnerar

Det nya add Slicer-index


```python
def add(self, pivot, row, column, base_field_name):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Pivottabellobjekt|
| row | int | Radindex för cellen i det övre vänstra hörnet av Slicer-området.|
| column | int | Kolumnindex för cellen i det övre vänstra hörnet av Slicer-intervallet.|
| base_field_name | str | Namnet på PivotField i PivotTable.BaseFields|

###  Exempel

```python

slicers.add(pivot, 20, 12, "fruit")

```


##  add(pivot, row, column, base_field_index) {#aspose.cells.pivot.PivotTable-int-int-int}
Lägg till en ny Slicer med pivottabell som datakälla


###  Returnerar

Det nya add Slicer-index


```python
def add(self, pivot, row, column, base_field_index):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Pivottabellobjekt|
| row | int | Radindex för cellen i det övre vänstra hörnet av Slicer-området.|
| column | int | Kolumnindex för cellen i det övre vänstra hörnet av Slicer-intervallet.|
| base_field_index | int | Indexet för PivotField i PivotTable.BaseFields|

###  Exempel

```python

slicers.add(pivot, 20, 8, 0)

```


##  add(pivot, row, column, base_field) {#aspose.cells.pivot.PivotTable-int-int-aspose.cells.pivot.PivotField}
Lägg till en ny Slicer med pivottabell som datakälla


###  Returnerar

Det nya add Slicer-index


```python
def add(self, pivot, row, column, base_field):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Pivottabellobjekt|
| row | int | Radindex för cellen i det övre vänstra hörnet av Slicer-området.|
| column | int | Kolumnindex för cellen i det övre vänstra hörnet av Slicer-intervallet.|
| base_field | aspose.cells.pivot.PivotField | Pivotfältet i PivotTable.BaseFields|

###  Exempel

```python

slicers.add(pivot, 3, 12, pivot.base_fields[0])

```


##  add(table, list_column, row, column) {#aspose.cells.tables.ListObject-aspose.cells.tables.ListColumn-int-int}
Lägg till en ny Slicer med ListObjet som datakälla


###  Returnerar

Det nya add Slicer-index


```python
def add(self, table, list_column, row, column):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| table | aspose.cells.tables.ListObject | ListObject-objekt|
| list_column | aspose.cells.tables.ListColumn | Listkolumnen i ListObject.ListColumns|
| row | int | Radindex för cellen i det övre vänstra hörnet av Slicer-området.|
| column | int | Kolumnindex för cellen i det övre vänstra hörnet av Slicer-intervallet.|

###  Exempel

```python

slicers.add(table, table.list_columns[1], 38, 12)

```



###  Se även
* modul [aspose.cells.slicers](../../)
* klass [SlicerCollection](/cells/sv/python-net/aspose.cells.slicers/slicercollection)
