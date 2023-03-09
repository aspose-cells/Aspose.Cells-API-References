---
title: add yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 20
url: /tr/python-net/aspose.cells.timelines/timelinecollection/add/
is_root: false
---
##  add(pivot, dest_cell_name, base_field_name) {#aspose.cells.pivot.PivotTable-str-str}
Veri kaynağı olarak PivotTable'ı kullanarak yeni bir Zaman Çizelgesi ekleyin


###  İadeler

Yeni add Zaman Çizelgesi dizini


```python
def add(self, pivot, dest_cell_name, base_field_name):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |PivotTable nesnesi|
| dest_cell_name | str | Zaman Çizelgesi aralığının sol üst köşesindeki hücre adı.|
| base_field_name | str | PivotTable.BaseFields içindeki PivotField'ın adı|

###  örnekler

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, "i15", "date")

```


##  add(pivot, dest_cell_name, base_field_index) {#aspose.cells.pivot.PivotTable-str-int}
Veri kaynağı olarak PivotTable'ı kullanarak yeni bir Zaman Çizelgesi ekleyin


###  İadeler

Yeni add Zaman Çizelgesi dizini


```python
def add(self, pivot, dest_cell_name, base_field_index):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |PivotTable nesnesi|
| dest_cell_name | str | Zaman Çizelgesi aralığının sol üst köşesindeki hücre adı.|
| base_field_index | int | PivotTable.BaseFields içindeki PivotField dizini|

###  örnekler

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, "i5", 1)

```


##  add(pivot, dest_cell_name, base_field) {#aspose.cells.pivot.PivotTable-str-aspose.cells.pivot.PivotField}
Veri kaynağı olarak PivotTable'ı kullanarak yeni bir Zaman Çizelgesi ekleyin


###  İadeler

Yeni add Zaman Çizelgesi dizini


```python
def add(self, pivot, dest_cell_name, base_field):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |PivotTable nesnesi|
| dest_cell_name | str | Zaman Çizelgesi aralığının sol üst köşesindeki hücre adı.|
| base_field | aspose.cells.pivot.PivotField | PivotTable.BaseFields içindeki PivotField|

###  örnekler

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, "i10", pivot.base_fields[1])

```


##  add(pivot, row, column, base_field_name) {#aspose.cells.pivot.PivotTable-int-int-str}
Veri kaynağı olarak PivotTable'ı kullanarak yeni bir Zaman Çizelgesi ekleyin


###  İadeler

Yeni add Zaman Çizelgesi dizini


```python
def add(self, pivot, row, column, base_field_name):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |PivotTable nesnesi|
| row | int | Zaman Çizelgesi aralığının sol üst köşesindeki hücrenin satır dizini.|
| column | int | Zaman Çizelgesi aralığının sol üst köşesindeki hücrenin sütun dizini.|
| base_field_name | str | PivotTable.BaseFields içindeki PivotField'ın adı|

###  örnekler

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, 10, 5, "date")

```


##  add(pivot, row, column, base_field_index) {#aspose.cells.pivot.PivotTable-int-int-int}
Veri kaynağı olarak PivotTable'ı kullanarak yeni bir Zaman Çizelgesi ekleyin


###  İadeler

Yeni add Zaman Çizelgesi dizini


```python
def add(self, pivot, row, column, base_field_index):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |PivotTable nesnesi|
| row | int | Zaman Çizelgesi aralığının sol üst köşesindeki hücrenin satır dizini.|
| column | int | Zaman Çizelgesi aralığının sol üst köşesindeki hücrenin sütun dizini.|
| base_field_index | int | PivotTable.BaseFields içindeki PivotField dizini|

###  örnekler

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, 15, 5, 1)

```


##  add(pivot, row, column, base_field) {#aspose.cells.pivot.PivotTable-int-int-aspose.cells.pivot.PivotField}
Veri kaynağı olarak PivotTable'ı kullanarak yeni bir Zaman Çizelgesi ekleyin


###  İadeler

Yeni add Zaman Çizelgesi dizini


```python
def add(self, pivot, row, column, base_field):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |PivotTable nesnesi|
| row | int | Zaman Çizelgesi aralığının sol üst köşesindeki hücrenin satır dizini.|
| column | int | Zaman Çizelgesi aralığının sol üst köşesindeki hücrenin sütun dizini.|
| base_field | aspose.cells.pivot.PivotField | PivotTable.BaseFields içindeki PivotField|

###  örnekler

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, 20, 5, pivot.base_fields[1])

```



###  Ayrıca bakınız
* modül [aspose.cells.timelines](../../)
* sınıf [TimelineCollection](/cells/tr/python-net/aspose.cells.timelines/timelinecollection)
