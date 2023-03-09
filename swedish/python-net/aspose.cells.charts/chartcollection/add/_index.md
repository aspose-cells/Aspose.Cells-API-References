---
title: add metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 20
url: /sv/python-net/aspose.cells.charts/chartcollection/add/
is_root: false
---
##  add(type, upper_left_row, upper_left_column, lower_right_row, lower_right_column) {#ChartType-int-int-int-int}
Lägger till ett diagram i samlingen.


###  Returnerar

[Chart](/cells/sv/python-net/aspose.cells.charts/chart) objektindex.


```python
def add(self, type, upper_left_row, upper_left_column, lower_right_row, lower_right_column):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| type | [ChartType](/cells/sv/python-net/aspose.cells.charts/charttype) | Diagramtyp|
| upper_left_row | int | Övre vänstra radens index.|
| upper_left_column | int |Övre vänstra kolumnindex.|
| lower_right_row | int | Nedre högra radindex|
| lower_right_column | int | Nedre högra kolumnindex|


##  add(type, data_range, top_row, left_column, right_row, bottom_column) {#ChartType-str-int-int-int-int}
Lägger till ett diagram i samlingen.


###  Returnerar

[Chart](/cells/sv/python-net/aspose.cells.charts/chart) objektindex.


```python
def add(self, type, data_range, top_row, left_column, right_row, bottom_column):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| type | [ChartType](/cells/sv/python-net/aspose.cells.charts/charttype) | Diagramtyp|
| data_range | str |Anger dataintervallet för diagrammet|
| top_row | int | Övre vänstra radens index.|
| left_column | int |Övre vänstra kolumnindex.|
| right_row | int | Nedre högra radindex|
| bottom_column | int | Nedre högra kolumnindex|
###  Anmärkningar

OBS: Denna medlem är nu föråldrad. Istället,
använd [ChartCollection.add(type, upper_left_row, upper_left_column, lower_right_row, lower_right_column)](/cells/sv/python-net/aspose.cells.charts/chartcollection/add) egendom.
Den här egenskapen kommer att tas bort 12 månader senare sedan maj 2022.
Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

##  add(data, data_range, is_vertical, top_row, left_column, right_row, bottom_column) {#bytes-str-bool-int-int-int-int}
Lägger till ett diagram med förinställd mall.


###  Returnerar

[Chart](/cells/sv/python-net/aspose.cells.charts/chart) objektindex.


```python
def add(self, data, data_range, is_vertical, top_row, left_column, right_row, bottom_column):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| data | bytes | Data för diagrammallfilen (.crtx).|
| data_range | str |Anger dataintervallet för diagrammet|
| is_vertical | bool | Anger om serien ska plottas från ett intervall av cellvärden efter rad eller kolumn.|
| top_row | int | Övre vänstra radens index.|
| left_column | int |Övre vänstra kolumnindex.|
| right_row | int | Nedre högra radindex|
| bottom_column | int | Nedre högra kolumnindex|


##  add(type, data_range, is_vertical, top_row, left_column, right_row, bottom_column) {#ChartType-str-bool-int-int-int-int}
Lägger till ett diagram i samlingen.


###  Returnerar

[Chart](/cells/sv/python-net/aspose.cells.charts/chart) objektindex.


```python
def add(self, type, data_range, is_vertical, top_row, left_column, right_row, bottom_column):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| type | [ChartType](/cells/sv/python-net/aspose.cells.charts/charttype) | Diagramtyp|
| data_range | str |Anger dataintervallet för diagrammet|
| is_vertical | bool | Anger om serien ska plottas från ett intervall av cellvärden efter rad eller kolumn.|
| top_row | int | Övre vänstra radens index.|
| left_column | int |Övre vänstra kolumnindex.|
| right_row | int | Nedre högra radindex|
| bottom_column | int | Nedre högra kolumnindex|



###  Se även
* modul [aspose.cells.charts](../../)
* klass [Chart](/cells/sv/python-net/aspose.cells.charts/chart)
* klass [ChartCollection](/cells/sv/python-net/aspose.cells.charts/chartcollection)
