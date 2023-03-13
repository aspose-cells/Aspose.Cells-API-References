---
title: set_array_formula Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 290
url: /de/python-net/aspose.cells/cell/set_array_formula/
is_root: false
---
##  set_array_formula(array_formula, row_number, column_number) {#str-int-int}
Legt eine Array-Formel (alte Array-Formel, die über STRG+UMSCHALT+EINGABETASTE in MS Excel eingegeben wurde) auf einen Bereich von Zellen fest.



```python
def set_array_formula(self, array_formula, row_number, column_number):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| array_formula | str | Array-Formel.|
| row_number | int |Anzahl der Zeilen zum Auffüllen des Ergebnisses der Matrixformel.|
| column_number | int | Anzahl der Spalten, die das Ergebnis der Matrixformel füllen sollen.|


##  set_array_formula(array_formula, row_number, column_number, options) {#str-int-int-FormulaParseOptions}
Legt eine Matrixformel auf einen Zellbereich fest.



```python
def set_array_formula(self, array_formula, row_number, column_number, options):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| array_formula | str | Array-Formel.|
| row_number | int |Anzahl der Zeilen zum Auffüllen des Ergebnisses der Matrixformel.|
| column_number | int | Anzahl der Spalten, die das Ergebnis der Matrixformel füllen sollen.|
| options | [FormulaParseOptions](/cells/de/python-net/aspose.cells/formulaparseoptions) | Optionen zum Analysieren der Formel.|


##  set_array_formula(array_formula, row_number, column_number, is_r1c1, is_local) {#str-int-int-bool-bool}
Legt eine Matrixformel auf einen Zellbereich fest.



```python
def set_array_formula(self, array_formula, row_number, column_number, is_r1c1, is_local):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| array_formula | str | Array-Formel.|
| row_number | int |Anzahl der Zeilen zum Auffüllen des Ergebnisses der Matrixformel.|
| column_number | int | Anzahl der Spalten, die das Ergebnis der Matrixformel füllen sollen.|
| is_r1c1 | bool | ob die Formel R1C1-Formel ist|
| is_local | bool | ob die Formel im Gebietsschema formatiert ist|
###  Bemerkungen

HINWEIS: Diese Klasse ist jetzt veraltet. Stattdessen,
verwenden Sie bitte Cell.SetArrayFormula(string,int,int,FormulaParseOptions).
Diese Property wird 12 Monate später seit Dezember 2019 entfernt.
Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

##  set_array_formula(array_formula, row_number, column_number, options, values) {#str-int-int-FormulaParseOptions-list}
Legt eine Matrixformel auf einen Zellbereich fest.



```python
def set_array_formula(self, array_formula, row_number, column_number, options, values):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| array_formula | str | Array-Formel.|
| row_number | int |Anzahl der Zeilen zum Auffüllen des Ergebnisses der Matrixformel.|
| column_number | int | Anzahl der Spalten, die das Ergebnis der Matrixformel füllen sollen.|
| options | [FormulaParseOptions](/cells/de/python-net/aspose.cells/formulaparseoptions) | Optionen zum Analysieren der Formel.|
| values | list | Werte für die Zellen mit gegebener Matrixformel|



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Cell](/cells/de/python-net/aspose.cells/cell)
