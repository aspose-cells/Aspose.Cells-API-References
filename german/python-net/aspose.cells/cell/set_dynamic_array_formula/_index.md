---
title: set_dynamic_array_formula Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 310
url: /de/python-net/aspose.cells/cell/set_dynamic_array_formula/
is_root: false
---
##  set_dynamic_array_formula(array_formula, options, calculate_value) {#str-FormulaParseOptions-bool}
Legt eine dynamische Matrixformel fest und lässt die Formel nach Möglichkeit in benachbarte Zellen übergehen.


###  Kehrt zurück

der Bereich, in den die Formel übergehen soll.


```python
def set_dynamic_array_formula(self, array_formula, options, calculate_value):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| array_formula | str | der Formelausdruck|
| options | [FormulaParseOptions](/cells/de/python-net/aspose.cells/formulaparseoptions) | Optionen zum Analysieren von Formeln.<br/> Die Option "Parsen" wird ignoriert und die Formel wird immer sofort analysiert|
| calculate_value | bool | ob diese dynamische Array-Formel für diese Zellen im verschütteten Bereich berechnet wird.|


##  set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value) {#str-FormulaParseOptions-list-bool-bool}
Legt eine dynamische Matrixformel fest und lässt die Formel nach Möglichkeit in benachbarte Zellen übergehen.


###  Kehrt zurück

der Bereich, in den die Formel übergehen soll.


```python
def set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| array_formula | str | der Formelausdruck|
| options | [FormulaParseOptions](/cells/de/python-net/aspose.cells/formulaparseoptions) | Optionen zum Analysieren von Formeln.<br/> Die Option "Parsen" wird ignoriert und die Formel wird immer sofort analysiert|
| values | list |Werte für diese Zellen mit gegebener dynamischer Matrixformel|
| calculate_range | bool | Ob der verschüttete Bereich für diese dynamische Matrixformel berechnet wird.<br/>Wenn der "Werte"-Parameter nicht null ist und dieses Flag falsch ist,<br/>dann ist die Höhe des verschütteten Bereichs values.Length und width sind values[0].Length.|
| calculate_value | bool | ob diese dynamische Array-Formel für die Zellen im verschütteten Bereich berechnet wird, wenn "values" null ist<br/> oder das entsprechende Element in "values" für eine Zelle ist null.|


##  set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value, copts) {#str-FormulaParseOptions-list-bool-bool-CalculationOptions}
Legt eine dynamische Matrixformel fest und lässt die Formel nach Möglichkeit in benachbarte Zellen übergehen.


###  Kehrt zurück

der Bereich, in den die Formel übergehen soll.


```python
def set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value, copts):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| array_formula | str | der Formelausdruck|
| options | [FormulaParseOptions](/cells/de/python-net/aspose.cells/formulaparseoptions) | Optionen zum Analysieren von Formeln.<br/> Die Option "Parsen" wird ignoriert und die Formel wird immer sofort analysiert|
| values | list |Werte für diese Zellen mit gegebener dynamischer Matrixformel|
| calculate_range | bool | Ob der verschüttete Bereich für diese dynamische Matrixformel berechnet wird.<br/>Wenn der "Werte"-Parameter nicht null ist und dieses Flag falsch ist,<br/>dann ist die Höhe des verschütteten Bereichs values.Length und width sind values[0].Length.|
| calculate_value | bool | ob diese dynamische Array-Formel für die Zellen im verschütteten Bereich berechnet wird, wenn "values" null ist<br/> oder das entsprechende Element in "values" für eine Zelle ist null.|
| copts | [CalculationOptions](/cells/de/python-net/aspose.cells/calculationoptions) | Die Optionen zur Berechnung der Formel.<br/> Im Allgemeinen sollte die Eigenschaft [CalculationOptions.recursive](/cells/de/python-net/aspose.cells/calculationoptions#recursive) aus Leistungsgründen falsch sein.|



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Cell](/cells/de/python-net/aspose.cells/cell)
