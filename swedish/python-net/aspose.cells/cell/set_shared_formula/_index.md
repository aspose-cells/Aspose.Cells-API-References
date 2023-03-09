---
title: set_shared_formula metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 330
url: /sv/python-net/aspose.cells/cell/set_shared_formula/
is_root: false
---
##  set_shared_formula(shared_formula, row_number, column_number) {#str-int-int}
Ställer in delade formler till ett cellintervall.



```python
def set_shared_formula(self, shared_formula, row_number, column_number):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| shared_formula | str | Delad formel.|
| row_number | int | Antal rader att fylla i formeln.|
| column_number | int | Antal kolumner att fylla i formeln.|
###  Anmärkningar



##  set_shared_formula(shared_formula, row_number, column_number, options) {#str-int-int-FormulaParseOptions}

Ställer in delade formler till ett cellintervall.



```python
def set_shared_formula(self, shared_formula, row_number, column_number, options):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| shared_formula | str | Delad formel.|
| row_number | int | Antal rader att fylla i formeln.|
| column_number | int | Antal kolumner att fylla i formeln.|
| options | [FormulaParseOptions](/cells/sv/python-net/aspose.cells/formulaparseoptions) | Alternativ för att analysera formeln.|


##  set_shared_formula(shared_formula, row_number, column_number, is_r1c1, is_local) {#str-int-int-bool-bool}
Ställer in en formel för ett cellintervall.



```python
def set_shared_formula(self, shared_formula, row_number, column_number, is_r1c1, is_local):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| shared_formula | str | Delad formel.|
| row_number | int | Antal rader att fylla i formeln.|
| column_number | int | Antal kolumner att fylla i formeln.|
| is_r1c1 | bool | om formeln är R1C1-formel|
| is_local | bool | om formeln är språkformaterad|
###  Anmärkningar

OBS: Denna klass är nu föråldrad. Istället,
använd Cell.SetSharedFormula(string,int,int,FormulaParseOptions).
Den här egenskapen kommer att tas bort 12 månader senare sedan december 2019.
Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

##  set_shared_formula(shared_formula, row_number, column_number, options, values) {#str-int-int-FormulaParseOptions-list}
Ställer in delade formler till ett cellintervall.



```python
def set_shared_formula(self, shared_formula, row_number, column_number, options, values):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| shared_formula | str | Delad formel.|
| row_number | int | Antal rader att fylla i formeln.|
| column_number | int | Antal kolumner att fylla i formeln.|
| options | [FormulaParseOptions](/cells/sv/python-net/aspose.cells/formulaparseoptions) | Alternativ för att analysera formeln.|
| values | list | värden för dessa celler med en given delad formel|



###  Se även
* modul [aspose.cells](../../)
* klass [Cell](/cells/sv/python-net/aspose.cells/cell)
