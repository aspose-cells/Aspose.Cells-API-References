---
title: add metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 20
url: /sv/python-net/aspose.cells.pivot/pivottablecollection/add/
is_root: false
---
##  add(source_data, dest_cell_name, table_name) {#str-str-str}
Lägger till en ny PivotTable-cache till en PivotCache-samling.


###  Returnerar

Det nya tillagda cacheindexet.


```python
def add(self, source_data, dest_cell_name, table_name):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| source_data | str | Data för den nya PivotTable-cachen.|
| dest_cell_name | str |Cellen i det övre vänstra hörnet av pivottabellrapportens målområde.|
| table_name | str | Namnet på den nya pivottabellsrapporten.|


##  add(pivot_table, dest_cell_name, table_name) {#PivotTable-str-str}
Lägger till ett nytt pivottabellobjekt till samlingen från en annan pivottabell.


###  Returnerar

Det nya tillagda pivottabellindexet.


```python
def add(self, pivot_table, dest_cell_name, table_name):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| pivot_table | [PivotTable](/cells/sv/python-net/aspose.cells.pivot/pivottable) | Källpivottabellen.|
| dest_cell_name | str |Cellen i det övre vänstra hörnet av pivottabellrapportens målområde.|
| table_name | str | Namnet på den nya pivottabellsrapporten.|


##  add(source_data, dest_cell_name, table_name, use_same_source) {#str-str-str-bool}
Lägger till en ny PivotTable-cache till en PivotCache-samling.


###  Returnerar

Det nya tillagda cacheindexet.


```python
def add(self, source_data, dest_cell_name, table_name, use_same_source):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| source_data | str | Data för den nya PivotTable-cachen.|
| dest_cell_name | str |Cellen i det övre vänstra hörnet av pivottabellrapportens målområde.|
| table_name | str | Namnet på den nya pivottabellsrapporten.|
| use_same_source | bool | Anger om samma datakälla används när en annan befintlig pivottabell har använt denna datakälla.<br/> Om egenskapen är sann kommer den att spara minne.|


##  add(source_data, row, column, table_name) {#str-int-int-str}
Lägger till en ny PivotTable-cache till en PivotCache-samling.


###  Returnerar

Det nya tillagda cacheindexet.


```python
def add(self, source_data, row, column, table_name):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| source_data | str | Datacellintervallet för den nya pivottabellen.Exempel: Blad1!A1:C8|
| row | int | Radindex för cellen i det övre vänstra hörnet av pivottabellrapportens målområde.|
| column | int | Kolumnindex för cellen i det övre vänstra hörnet av pivottabellrapportens målområde.|
| table_name | str | Namnet på den nya pivottabellsrapporten.|


##  add(pivot_table, row, column, table_name) {#PivotTable-int-int-str}
Lägger till ett nytt pivottabellobjekt till samlingen från en annan pivottabell.


###  Returnerar

Det nya tillagda pivottabellindexet.


```python
def add(self, pivot_table, row, column, table_name):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| pivot_table | [PivotTable](/cells/sv/python-net/aspose.cells.pivot/pivottable) | Källpivottabellen.|
| row | int | Radindex för cellen i det övre vänstra hörnet av pivottabellrapportens målområde.|
| column | int | Kolumnindex för cellen i det övre vänstra hörnet av pivottabellrapportens målområde.|
| table_name | str | Namnet på den nya pivottabellsrapporten.|


##  add(source_data, row, column, table_name, use_same_source) {#str-int-int-str-bool}
Lägger till en ny PivotTable-cache till en PivotCache-samling.


###  Returnerar

Det nya tillagda cacheindexet.


```python
def add(self, source_data, row, column, table_name, use_same_source):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| source_data | str | Datacellintervallet för den nya pivottabellen.Exempel: Blad1!A1:C8|
| row | int | Radindex för cellen i det övre vänstra hörnet av pivottabellrapportens målområde.|
| column | int | Kolumnindex för cellen i det övre vänstra hörnet av pivottabellrapportens målområde.|
| table_name | str | Namnet på den nya pivottabellsrapporten.|
| use_same_source | bool | Anger om samma datakälla används när en annan befintlig pivottabell har använt denna datakälla.<br/> Om egenskapen är sann kommer den att spara minne.|


##  add(source_data, is_auto_page, page_fields, dest_cell_name, table_name) {#list-bool-PivotPageFields-str-str}
Lägger till ett nytt pivottabellobjekt till samlingen med flera konsolideringsintervall som datakälla.


###  Returnerar

Det nya tillagda pivottabellindexet.


```python
def add(self, source_data, is_auto_page, page_fields, dest_cell_name, table_name):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| source_data | list | De flera konsolideringsintervallen, såsom {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| is_auto_page | bool | Huruvida automatiskt skapa ett ensidfält.<br/>Om sant, kommer följande param pageFields att ignoreras.|
| page_fields | [PivotPageFields](/cells/sv/python-net/aspose.cells.pivot/pivotpagefields) | Pivotsidans fältobjekt.|
| dest_cell_name | str | destCellName Namnet på den nya pivottabellsrapporten.|
| table_name | str | namnet på den nya pivottabellsrapporten.|


##  add(source_data, is_auto_page, page_fields, row, column, table_name) {#list-bool-PivotPageFields-int-int-str}
Lägger till ett nytt pivottabellobjekt till samlingen med flera konsolideringsintervall som datakälla.


###  Returnerar

Det nya tillagda pivottabellindexet.


```python
def add(self, source_data, is_auto_page, page_fields, row, column, table_name):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| source_data | list | De flera konsolideringsintervallen, såsom {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| is_auto_page | bool | Huruvida automatiskt skapa ett ensidfält.<br/> Om sant, kommer följande param pageFields att ignoreras|
| page_fields | [PivotPageFields](/cells/sv/python-net/aspose.cells.pivot/pivotpagefields) | Pivotsidans fältobjekt.|
| row | int | Radindex för cellen i det övre vänstra hörnet av pivottabellrapportens målområde.|
| column | int | Kolumnindex för cellen i det övre vänstra hörnet av pivottabellrapportens målområde.|
| table_name | str | Namnet på den nya pivottabellsrapporten.|



###  Se även
* modul [aspose.cells.pivot](../../)
* klass [PivotTableCollection](/cells/sv/python-net/aspose.cells.pivot/pivottablecollection)
