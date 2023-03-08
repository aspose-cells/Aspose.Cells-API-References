---
title: add Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 20
url: /de/python-net/aspose.cells.pivot/pivottablecollection/add/
is_root: false
---
##  add(source_data, dest_cell_name, table_name) {#str-str-str}
Fügt einer PivotCaches-Auflistung einen neuen PivotTable-Cache hinzu.


###  Kehrt zurück

Der neu hinzugefügte Cache-Index.


```python
def add(self, source_data, dest_cell_name, table_name):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| source_data | str | Die Daten für den neuen PivotTable-Cache.|
| dest_cell_name | str | Die Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts.|
| table_name | str | Der Name des neuen PivotTable-Berichts.|


##  add(pivot_table, dest_cell_name, table_name) {#PivotTable-str-str}
Fügt der Auflistung ein neues PivotTable-Objekt aus einer anderen PivotTable hinzu.


###  Kehrt zurück

Der neu hinzugefügte PivotTable-Index.


```python
def add(self, pivot_table, dest_cell_name, table_name):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| pivot_table | [PivotTable](/cells/de/python-net/aspose.cells.pivot/pivottable) | Die Quell-PivotTable.|
| dest_cell_name | str | Die Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts.|
| table_name | str | Der Name des neuen PivotTable-Berichts.|


##  add(source_data, dest_cell_name, table_name, use_same_source) {#str-str-str-bool}
Fügt einer PivotCaches-Auflistung einen neuen PivotTable-Cache hinzu.


###  Kehrt zurück

Der neu hinzugefügte Cache-Index.


```python
def add(self, source_data, dest_cell_name, table_name, use_same_source):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| source_data | str | Die Daten für den neuen PivotTable-Cache.|
| dest_cell_name | str | Die Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts.|
| table_name | str | Der Name des neuen PivotTable-Berichts.|
| use_same_source | bool | Gibt an, ob dieselbe Datenquelle verwendet wird, wenn eine andere vorhandene Pivot-Tabelle diese Datenquelle verwendet hat.<br/> Wenn die Eigenschaft wahr ist, wird Speicher gespart.|


##  add(source_data, row, column, table_name) {#str-int-int-str}
Fügt einer PivotCaches-Auflistung einen neuen PivotTable-Cache hinzu.


###  Kehrt zurück

Der neu hinzugefügte Cache-Index.


```python
def add(self, source_data, row, column, table_name):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| source_data | str | Der Datenzellenbereich für die neue PivotTable.Example : Sheet1!A1:C8|
| row | int | Zeilenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts.|
| column | int | Spaltenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts.|
| table_name | str | Der Name des neuen PivotTable-Berichts.|


##  add(pivot_table, row, column, table_name) {#PivotTable-int-int-str}
Fügt der Auflistung ein neues PivotTable-Objekt aus einer anderen PivotTable hinzu.


###  Kehrt zurück

Der neu hinzugefügte PivotTable-Index.


```python
def add(self, pivot_table, row, column, table_name):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| pivot_table | [PivotTable](/cells/de/python-net/aspose.cells.pivot/pivottable) | Die Quell-PivotTable.|
| row | int | Zeilenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts.|
| column | int | Spaltenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts.|
| table_name | str | Der Name des neuen PivotTable-Berichts.|


##  add(source_data, row, column, table_name, use_same_source) {#str-int-int-str-bool}
Fügt einer PivotCaches-Auflistung einen neuen PivotTable-Cache hinzu.


###  Kehrt zurück

Der neu hinzugefügte Cache-Index.


```python
def add(self, source_data, row, column, table_name, use_same_source):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| source_data | str | Der Datenzellenbereich für die neue PivotTable.Example : Sheet1!A1:C8|
| row | int | Zeilenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts.|
| column | int | Spaltenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts.|
| table_name | str | Der Name des neuen PivotTable-Berichts.|
| use_same_source | bool | Gibt an, ob dieselbe Datenquelle verwendet wird, wenn eine andere vorhandene Pivot-Tabelle diese Datenquelle verwendet hat.<br/> Wenn die Eigenschaft wahr ist, wird Speicher gespart.|


##  add(source_data, is_auto_page, page_fields, dest_cell_name, table_name) {#list-bool-PivotPageFields-str-str}
Fügt der Sammlung ein neues PivotTable-Objekt mit mehreren Konsolidierungsbereichen als Datenquelle hinzu.


###  Kehrt zurück

Der neu hinzugefügte PivotTable-Index.


```python
def add(self, source_data, is_auto_page, page_fields, dest_cell_name, table_name):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| source_data | list | Die mehreren Konsolidierungsbereiche, z. B. {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| is_auto_page | bool | Ob ein einzelnes Seitenfeld automatisch erstellt wird.<br/> Wenn wahr, werden die folgenden Parameterseitenfelder ignoriert.|
| page_fields | [PivotPageFields](/cells/de/python-net/aspose.cells.pivot/pivotpagefields) | Die Feldelemente der Pivot-Seite.|
| dest_cell_name | str | destCellName Der Name des neuen PivotTable-Berichts.|
| table_name | str | der Name des neuen PivotTable-Berichts.|


##  add(source_data, is_auto_page, page_fields, row, column, table_name) {#list-bool-PivotPageFields-int-int-str}
Fügt der Sammlung ein neues PivotTable-Objekt mit mehreren Konsolidierungsbereichen als Datenquelle hinzu.


###  Kehrt zurück

Der neu hinzugefügte PivotTable-Index.


```python
def add(self, source_data, is_auto_page, page_fields, row, column, table_name):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| source_data | list | Die mehreren Konsolidierungsbereiche, z. B. {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| is_auto_page | bool | Ob ein einzelnes Seitenfeld automatisch erstellt wird.<br/> Wenn wahr, werden die folgenden Parameterseitenfelder ignoriert|
| page_fields | [PivotPageFields](/cells/de/python-net/aspose.cells.pivot/pivotpagefields) | Die Feldelemente der Pivot-Seite.|
| row | int | Zeilenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts.|
| column | int | Spaltenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts.|
| table_name | str | Der Name des neuen PivotTable-Berichts.|



###  Siehe auch
* Modul [aspose.cells.pivot](../../)
* Klasse [PivotTableCollection](/cells/de/python-net/aspose.cells.pivot/pivottablecollection)
