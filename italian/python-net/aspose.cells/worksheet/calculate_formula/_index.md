---
title: metodo calculate_formula
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 80
url: /it/python-net/aspose.cells/worksheet/calculate_formula/
is_root: false
---
##  calculate_formula(formula) {#str}
Calcola una formula.


###  ritorna

Risultato della formula calcolata.


```python
def calculate_formula(self, formula):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| formula | str | Formula da calcolare.|


##  calculate_formula(formula, opts) {#str-CalculationOptions}
Calcola una formula.


###  ritorna

Risultato della formula calcolata.


```python
def calculate_formula(self, formula, opts):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| formula | str | Formula da calcolare.|
| opts | [CalculationOptions](/cells/it/python-net/aspose.cells/calculationoptions) | Opzioni per il calcolo della formula|


##  calculate_formula(options, recursive) {#CalculationOptions-bool}
Calcola tutte le formule in questo foglio di lavoro.



```python
def calculate_formula(self, options, recursive):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| options | [CalculationOptions](/cells/it/python-net/aspose.cells/calculationoptions) | Opzioni per il calcolo|
| recursive | bool | Vero significa che se le celle del foglio di lavoro dipendono dalle celle di altri fogli di lavoro,<br/>verranno calcolate anche le celle dipendenti in altri fogli di lavoro.<br/> Falso significa che tutte le formule nel foglio di lavoro sono state calcolate e i valori sono corretti.|


##  calculate_formula(recursive, ignore_error, custom_function) {#bool-bool-ICustomFunction}
Calcola tutte le formule in questo foglio di lavoro.



```python
def calculate_formula(self, recursive, ignore_error, custom_function):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| recursive | bool | Vero significa che se le celle del foglio di lavoro dipendono dalle celle di altri fogli di lavoro,<br/>verranno calcolate anche le celle dipendenti in altri fogli di lavoro.<br/> Falso significa che tutte le formule nel foglio di lavoro sono state calcolate e i valori sono corretti.|
| ignore_error | bool | Indica se nascondere l'errore nel calcolo delle formule.<br/> L'errore potrebbe essere una funzione non supportata, collegamenti esterni, ecc.|
| custom_function | [ICustomFunction](/cells/it/python-net/aspose.cells/icustomfunction) | Il calcolo della formula personalizzata funziona per estendere il motore di calcolo.|
###  Osservazioni

NOTA: questo membro è ora obsoleto. Invece,
si prega di utilizzare il metodo CalculateFormula(CalculationOptions, bool).
 Questo metodo verrà rimosso 12 mesi dopo da agosto 2020.
Aspose si scusa per gli eventuali disagi causati.


###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Worksheet](/cells/it/python-net/aspose.cells/worksheet)
