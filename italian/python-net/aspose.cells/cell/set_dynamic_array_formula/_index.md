---
title: metodo set_dynamic_array_formula
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 310
url: /it/python-net/aspose.cells/cell/set_dynamic_array_formula/
is_root: false
---
##  set_dynamic_array_formula(array_formula, options, calculate_value) {#str-FormulaParseOptions-bool}
Imposta la formula di matrice dinamica e fa sì che la formula si riversi nelle celle vicine, se possibile.


###  ritorna

l'intervallo in cui la formula dovrebbe riversarsi.


```python
def set_dynamic_array_formula(self, array_formula, options, calculate_value):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| array_formula | str | l'espressione della formula|
| options | [FormulaParseOptions](/cells/it/python-net/aspose.cells/formulaparseoptions) | opzioni per analizzare la formula.<br/> L'opzione "Parse" verrà ignorata e la formula verrà sempre analizzata immediatamente|
| calculate_value | bool | se calcolare questa formula di matrice dinamica per quelle celle nell'intervallo versato.|


##  set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value) {#str-FormulaParseOptions-list-bool-bool}
Imposta la formula di matrice dinamica e fa sì che la formula si riversi nelle celle vicine, se possibile.


###  ritorna

l'intervallo in cui la formula dovrebbe riversarsi.


```python
def set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| array_formula | str | l'espressione della formula|
| options | [FormulaParseOptions](/cells/it/python-net/aspose.cells/formulaparseoptions) | opzioni per analizzare la formula.<br/> L'opzione "Parse" verrà ignorata e la formula verrà sempre analizzata immediatamente|
| values | list |valori per quelle celle con una data formula di matrice dinamica|
| calculate_range | bool | Indica se calcolare l'intervallo versato per questa formula di matrice dinamica.<br/>Se il parametro "values" non è nullo e questo flag è false,<br/> quindi l'altezza dell'intervallo versato sarà valori. Lunghezza e larghezza saranno valori[0].Length.|
| calculate_value | bool | se calcolare questa formula di matrice dinamica per quelle celle nell'intervallo versato quando "valori" è nullo<br/> o l'elemento corrispondente in "valori" per una cella è nullo.|


##  set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value, copts) {#str-FormulaParseOptions-list-bool-bool-CalculationOptions}
Imposta la formula di matrice dinamica e fa sì che la formula si riversi nelle celle vicine, se possibile.


###  ritorna

l'intervallo in cui la formula dovrebbe riversarsi.


```python
def set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value, copts):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| array_formula | str | l'espressione della formula|
| options | [FormulaParseOptions](/cells/it/python-net/aspose.cells/formulaparseoptions) | opzioni per analizzare la formula.<br/> L'opzione "Parse" verrà ignorata e la formula verrà sempre analizzata immediatamente|
| values | list |valori per quelle celle con una data formula di matrice dinamica|
| calculate_range | bool | Indica se calcolare l'intervallo versato per questa formula di matrice dinamica.<br/>Se il parametro "values" non è nullo e questo flag è false,<br/> quindi l'altezza dell'intervallo versato sarà valori. Lunghezza e larghezza saranno valori[0].Length.|
| calculate_value | bool | se calcolare questa formula di matrice dinamica per quelle celle nell'intervallo versato quando "valori" è nullo<br/> o l'elemento corrispondente in "valori" per una cella è nullo.|
| copts | [CalculationOptions](/cells/it/python-net/aspose.cells/calculationoptions) | Le opzioni per il calcolo della formula.<br/> In genere, per considerazioni sulle prestazioni, la proprietà [CalculationOptions.recursive](/cells/it/python-net/aspose.cells/calculationoptions#recursive) dovrebbe essere false.|



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Cell](/cells/it/python-net/aspose.cells/cell)
