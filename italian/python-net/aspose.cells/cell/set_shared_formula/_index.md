---
title: metodo set_shared_formula
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 330
url: /it/python-net/aspose.cells/cell/set_shared_formula/
is_root: false
---
##  set_shared_formula(shared_formula, row_number, column_number) {#str-int-int}
Imposta le formule condivise su un intervallo di celle.



```python
def set_shared_formula(self, shared_formula, row_number, column_number):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| shared_formula | str | Formula condivisa.|
| row_number | int |Numero di righe per popolare la formula.|
| column_number | int | Numero di colonne per popolare la formula.|
###  Osservazioni



##  set_shared_formula(shared_formula, row_number, column_number, options) {#str-int-int-FormulaParseOptions}

Imposta le formule condivise su un intervallo di celle.



```python
def set_shared_formula(self, shared_formula, row_number, column_number, options):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| shared_formula | str | Formula condivisa.|
| row_number | int |Numero di righe per popolare la formula.|
| column_number | int | Numero di colonne per popolare la formula.|
| options | [FormulaParseOptions](/cells/it/python-net/aspose.cells/formulaparseoptions) | Opzioni per l'analisi della formula.|


##  set_shared_formula(shared_formula, row_number, column_number, is_r1c1, is_local) {#str-int-int-bool-bool}
Imposta una formula su un intervallo di celle.



```python
def set_shared_formula(self, shared_formula, row_number, column_number, is_r1c1, is_local):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| shared_formula | str | Formula condivisa.|
| row_number | int |Numero di righe per popolare la formula.|
| column_number | int | Numero di colonne per popolare la formula.|
| is_r1c1 | bool | se la formula è la formula R1C1|
| is_local | bool | se la formula è in formato locale|
###  Osservazioni

NOTA: questa classe è ora obsoleta. Invece,
si prega di utilizzare Cell.SetSharedFormula(string,int,int,FormulaParseOptions).
Questa proprietà verrà rimossa 12 mesi dopo da dicembre 2019.
Aspose si scusa per gli eventuali disagi causati.

##  set_shared_formula(shared_formula, row_number, column_number, options, values) {#str-int-int-FormulaParseOptions-list}
Imposta le formule condivise su un intervallo di celle.



```python
def set_shared_formula(self, shared_formula, row_number, column_number, options, values):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| shared_formula | str | Formula condivisa.|
| row_number | int |Numero di righe per popolare la formula.|
| column_number | int | Numero di colonne per popolare la formula.|
| options | [FormulaParseOptions](/cells/it/python-net/aspose.cells/formulaparseoptions) | Opzioni per l'analisi della formula.|
| values | list | valori per quelle celle con una data formula condivisa|



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Cell](/cells/it/python-net/aspose.cells/cell)
