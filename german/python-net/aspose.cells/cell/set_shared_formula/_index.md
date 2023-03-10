---
title: set_shared_formula Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 330
url: /de/python-net/aspose.cells/cell/set_shared_formula/
is_root: false
---
##  set_shared_formula(shared_formula, row_number, column_number) {#str-int-int}
Legt freigegebene Formeln auf einen Zellbereich fest.



```python
def set_shared_formula(self, shared_formula, row_number, column_number):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| shared_formula | str | Geteilte Formel.|
| row_number | int |Anzahl der Zeilen zum Ausfüllen der Formel.|
| column_number | int | Anzahl der Spalten zum Ausfüllen der Formel.|
###  Bemerkungen



##  set_shared_formula(shared_formula, row_number, column_number, options) {#str-int-int-FormulaParseOptions}

Legt freigegebene Formeln auf einen Zellbereich fest.



```python
def set_shared_formula(self, shared_formula, row_number, column_number, options):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| shared_formula | str | Geteilte Formel.|
| row_number | int |Anzahl der Zeilen zum Ausfüllen der Formel.|
| column_number | int | Anzahl der Spalten zum Ausfüllen der Formel.|
| options | [FormulaParseOptions](/cells/de/python-net/aspose.cells/formulaparseoptions) | Optionen zum Analysieren der Formel.|


##  set_shared_formula(shared_formula, row_number, column_number, is_r1c1, is_local) {#str-int-int-bool-bool}
Legt eine Formel auf einen Zellbereich fest.



```python
def set_shared_formula(self, shared_formula, row_number, column_number, is_r1c1, is_local):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| shared_formula | str | Geteilte Formel.|
| row_number | int |Anzahl der Zeilen zum Ausfüllen der Formel.|
| column_number | int | Anzahl der Spalten zum Ausfüllen der Formel.|
| is_r1c1 | bool | ob die Formel R1C1-Formel ist|
| is_local | bool | ob die Formel im Gebietsschema formatiert ist|
###  Bemerkungen

HINWEIS: Diese Klasse ist jetzt veraltet. Stattdessen,
verwenden Sie bitte Cell.SetSharedFormula(string,int,int,FormulaParseOptions).
Diese Property wird 12 Monate später seit Dezember 2019 entfernt.
Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

##  set_shared_formula(shared_formula, row_number, column_number, options, values) {#str-int-int-FormulaParseOptions-list}
Legt freigegebene Formeln auf einen Zellbereich fest.



```python
def set_shared_formula(self, shared_formula, row_number, column_number, options, values):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| shared_formula | str | Geteilte Formel.|
| row_number | int |Anzahl der Zeilen zum Ausfüllen der Formel.|
| column_number | int | Anzahl der Spalten zum Ausfüllen der Formel.|
| options | [FormulaParseOptions](/cells/de/python-net/aspose.cells/formulaparseoptions) | Optionen zum Analysieren der Formel.|
| values | list | Werte für die Zellen mit der angegebenen gemeinsamen Formel|



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Cell](/cells/de/python-net/aspose.cells/cell)
