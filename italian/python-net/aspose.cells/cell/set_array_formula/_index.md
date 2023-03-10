---
title: metodo set_array_formula
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 290
url: /it/python-net/aspose.cells/cell/set_array_formula/
is_root: false
---
##  set_array_formula(array_formula, row_number, column_number) {#str-int-int}
Imposta una formula di matrice (formula di matrice legacy immessa tramite CTRL+MAIUSC+INVIO in ms excel) su un intervallo di celle.



```python
def set_array_formula(self, array_formula, row_number, column_number):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| array_formula | str | Formula matrice.|
| row_number | int |Numero di righe da popolare risultato della formula di matrice.|
| column_number | int | Numero di colonne da popolare risultato della formula di matrice.|


##  set_array_formula(array_formula, row_number, column_number, options) {#str-int-int-FormulaParseOptions}
Imposta una formula di matrice su un intervallo di celle.



```python
def set_array_formula(self, array_formula, row_number, column_number, options):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| array_formula | str | Formula matrice.|
| row_number | int |Numero di righe da popolare risultato della formula di matrice.|
| column_number | int | Numero di colonne da popolare risultato della formula di matrice.|
| options | [FormulaParseOptions](/cells/it/python-net/aspose.cells/formulaparseoptions) | Opzioni per l'analisi della formula.|


##  set_array_formula(array_formula, row_number, column_number, is_r1c1, is_local) {#str-int-int-bool-bool}
Imposta una formula di matrice su un intervallo di celle.



```python
def set_array_formula(self, array_formula, row_number, column_number, is_r1c1, is_local):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| array_formula | str | Formula matrice.|
| row_number | int |Numero di righe da popolare risultato della formula di matrice.|
| column_number | int | Numero di colonne da popolare risultato della formula di matrice.|
| is_r1c1 | bool | se la formula è la formula R1C1|
| is_local | bool | se la formula è in formato locale|
###  Osservazioni

NOTA: questa classe è ora obsoleta. Invece,
si prega di utilizzare Cell.SetArrayFormula(string,int,int,FormulaParseOptions).
Questa proprietà verrà rimossa 12 mesi dopo da dicembre 2019.
Aspose si scusa per gli eventuali disagi causati.

##  set_array_formula(array_formula, row_number, column_number, options, values) {#str-int-int-FormulaParseOptions-list}
Imposta una formula di matrice su un intervallo di celle.



```python
def set_array_formula(self, array_formula, row_number, column_number, options, values):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| array_formula | str | Formula matrice.|
| row_number | int |Numero di righe da popolare risultato della formula di matrice.|
| column_number | int | Numero di colonne da popolare risultato della formula di matrice.|
| options | [FormulaParseOptions](/cells/it/python-net/aspose.cells/formulaparseoptions) | Opzioni per l'analisi della formula.|
| values | list | valori per quelle celle con una data formula di matrice|



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Cell](/cells/it/python-net/aspose.cells/cell)
