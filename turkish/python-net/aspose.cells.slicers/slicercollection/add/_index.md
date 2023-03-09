---
title: add yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 20
url: /tr/python-net/aspose.cells.slicers/slicercollection/add/
is_root: false
---
##  add(pivot, dest_cell_name, base_field_name) {#aspose.cells.pivot.PivotTable-str-str}
Veri kaynağı olarak PivotTable'ı kullanarak yeni bir Dilimleyici ekleyin


###  İadeler

Yeni add Dilimleyici dizini


```python
def add(self, pivot, dest_cell_name, base_field_name):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |PivotTable nesnesi|
| dest_cell_name | str | Dilimleyici aralığının sol üst köşesindeki hücre.|
| base_field_name | str | PivotTable.BaseFields içindeki PivotField'ın adı|

###  örnekler

```python

slicers.add(pivot, "E3", "fruit")

```


##  add(pivot, dest_cell_name, base_field_index) {#aspose.cells.pivot.PivotTable-str-int}
Veri kaynağı olarak PivotTable'ı kullanarak yeni bir Dilimleyici ekleyin


###  İadeler

Yeni add Dilimleyici dizini


```python
def add(self, pivot, dest_cell_name, base_field_index):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |PivotTable nesnesi|
| dest_cell_name | str | Dilimleyici aralığının sol üst köşesindeki hücre.|
| base_field_index | int | PivotTable.BaseFields içindeki PivotField dizini|

###  örnekler

```python

slicers.add(pivot, "E20", 0)

```


##  add(pivot, dest_cell_name, base_field) {#aspose.cells.pivot.PivotTable-str-aspose.cells.pivot.PivotField}
Veri kaynağı olarak PivotTable'ı kullanarak yeni bir Dilimleyici ekleyin


###  İadeler

Yeni add Dilimleyici dizini


```python
def add(self, pivot, dest_cell_name, base_field):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |PivotTable nesnesi|
| dest_cell_name | str | Dilimleyici aralığının sol üst köşesindeki hücre.|
| base_field | aspose.cells.pivot.PivotField | PivotTable.BaseFields içindeki PivotField|

###  örnekler

```python

slicers.add(pivot, "I3", pivot.base_fields[0])

```


##  add(table, index, dest_cell_name) {#aspose.cells.tables.ListObject-int-str}
Veri kaynağı olarak ListObjet kullanarak yeni bir Dilimleyici ekleyin


###  İadeler

Yeni add Dilimleyici dizini


```python
def add(self, table, index, dest_cell_name):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| table | aspose.cells.tables.ListObject | ListObject nesnesi|
| index | int | ListObject.ListColumns içindeki ListColumn dizini|
| dest_cell_name | str | Dilimleyici aralığının sol üst köşesindeki hücre.|

###  örnekler

```python

slicers.add(table, 1, "E38")

```


##  add(table, list_column, dest_cell_name) {#aspose.cells.tables.ListObject-aspose.cells.tables.ListColumn-str}
Veri kaynağı olarak ListObjet kullanarak yeni bir Dilimleyici ekleyin


###  İadeler

Yeni add Dilimleyici dizini


```python
def add(self, table, list_column, dest_cell_name):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| table | aspose.cells.tables.ListObject | ListObject nesnesi|
| list_column | aspose.cells.tables.ListColumn | ListObject.ListColumns içindeki ListColumn|
| dest_cell_name | str | Dilimleyici aralığının sol üst köşesindeki hücre.|

###  örnekler

```python

slicers.add(table, table.list_columns[1], "I38")

```


##  add(pivot, row, column, base_field_name) {#aspose.cells.pivot.PivotTable-int-int-str}
Veri kaynağı olarak PivotTable'ı kullanarak yeni bir Dilimleyici ekleyin


###  İadeler

Yeni add Dilimleyici dizini


```python
def add(self, pivot, row, column, base_field_name):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |PivotTable nesnesi|
| row | int | Dilimleyici aralığının sol üst köşesindeki hücrenin satır dizini.|
| column | int | Dilimleyici aralığının sol üst köşesindeki hücrenin sütun dizini.|
| base_field_name | str | PivotTable.BaseFields içindeki PivotField'ın adı|

###  örnekler

```python

slicers.add(pivot, 20, 12, "fruit")

```


##  add(pivot, row, column, base_field_index) {#aspose.cells.pivot.PivotTable-int-int-int}
Veri kaynağı olarak PivotTable'ı kullanarak yeni bir Dilimleyici ekleyin


###  İadeler

Yeni add Dilimleyici dizini


```python
def add(self, pivot, row, column, base_field_index):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |PivotTable nesnesi|
| row | int | Dilimleyici aralığının sol üst köşesindeki hücrenin satır dizini.|
| column | int | Dilimleyici aralığının sol üst köşesindeki hücrenin sütun dizini.|
| base_field_index | int | PivotTable.BaseFields içindeki PivotField dizini|

###  örnekler

```python

slicers.add(pivot, 20, 8, 0)

```


##  add(pivot, row, column, base_field) {#aspose.cells.pivot.PivotTable-int-int-aspose.cells.pivot.PivotField}
Veri kaynağı olarak PivotTable'ı kullanarak yeni bir Dilimleyici ekleyin


###  İadeler

Yeni add Dilimleyici dizini


```python
def add(self, pivot, row, column, base_field):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |PivotTable nesnesi|
| row | int | Dilimleyici aralığının sol üst köşesindeki hücrenin satır dizini.|
| column | int | Dilimleyici aralığının sol üst köşesindeki hücrenin sütun dizini.|
| base_field | aspose.cells.pivot.PivotField | PivotTable.BaseFields içindeki PivotField|

###  örnekler

```python

slicers.add(pivot, 3, 12, pivot.base_fields[0])

```


##  add(table, list_column, row, column) {#aspose.cells.tables.ListObject-aspose.cells.tables.ListColumn-int-int}
Veri kaynağı olarak ListObjet kullanarak yeni bir Dilimleyici ekleyin


###  İadeler

Yeni add Dilimleyici dizini


```python
def add(self, table, list_column, row, column):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| table | aspose.cells.tables.ListObject | ListObject nesnesi|
| list_column | aspose.cells.tables.ListColumn | ListObject.ListColumns içindeki ListColumn|
| row | int | Dilimleyici aralığının sol üst köşesindeki hücrenin satır dizini.|
| column | int | Dilimleyici aralığının sol üst köşesindeki hücrenin sütun dizini.|

###  örnekler

```python

slicers.add(table, table.list_columns[1], 38, 12)

```



###  Ayrıca bakınız
* modül [aspose.cells.slicers](../../)
* sınıf [SlicerCollection](/cells/tr/python-net/aspose.cells.slicers/slicercollection)
