---
title: set_dynamic_array_formula metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 310
url: /sv/python-net/aspose.cells/cell/set_dynamic_array_formula/
is_root: false
---
##  set_dynamic_array_formula(array_formula, options, calculate_value) {#str-FormulaParseOptions-bool}
Ställer in dynamisk matrisformel och får formeln att spilla in i närliggande celler om möjligt.


###  Returnerar

intervallet som formeln ska spilla in i.


```python
def set_dynamic_array_formula(self, array_formula, options, calculate_value):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| array_formula | str | formeluttrycket|
| options | [FormulaParseOptions](/cells/sv/python-net/aspose.cells/formulaparseoptions) | alternativ för att analysera formel.<br/> Alternativet "Parse" kommer att ignoreras och formeln kommer alltid att analyseras omedelbart|
| calculate_value | bool | om beräkna denna dynamiska matrisformel för de cellerna i det utspillda området.|


##  set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value) {#str-FormulaParseOptions-list-bool-bool}
Ställer in dynamisk matrisformel och får formeln att spilla in i närliggande celler om möjligt.


###  Returnerar

intervallet som formeln ska spilla in i.


```python
def set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| array_formula | str | formeluttrycket|
| options | [FormulaParseOptions](/cells/sv/python-net/aspose.cells/formulaparseoptions) | alternativ för att analysera formel.<br/> Alternativet "Parse" kommer att ignoreras och formeln kommer alltid att analyseras omedelbart|
| values | list |värden för dessa celler med given dynamisk matrisformel|
| calculate_range | bool | Beräkna det utspillda intervallet för denna dynamiska matrisformel.<br/>Om parametern "values" inte är null och denna flagga är falsk,<br/> då blir det utspillda områdets höjd värden. Längd och bredd kommer att vara värden[0].Längd.|
| calculate_value | bool | om beräkna denna dynamiska matrisformel för de cellerna i det utspillda området när "värden" är null<br/> eller motsvarande objekt i "värden" för en cell är null.|


##  set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value, copts) {#str-FormulaParseOptions-list-bool-bool-CalculationOptions}
Ställer in dynamisk matrisformel och får formeln att spilla in i närliggande celler om möjligt.


###  Returnerar

intervallet som formeln ska spilla in i.


```python
def set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value, copts):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| array_formula | str | formeluttrycket|
| options | [FormulaParseOptions](/cells/sv/python-net/aspose.cells/formulaparseoptions) | alternativ för att analysera formel.<br/> Alternativet "Parse" kommer att ignoreras och formeln kommer alltid att analyseras omedelbart|
| values | list |värden för dessa celler med given dynamisk matrisformel|
| calculate_range | bool | Beräkna det utspillda intervallet för denna dynamiska matrisformel.<br/>Om parametern "values" inte är null och denna flagga är falsk,<br/> då blir det utspillda områdets höjd värden. Längd och bredd kommer att vara värden[0].Längd.|
| calculate_value | bool | om beräkna denna dynamiska matrisformel för de cellerna i det utspillda området när "värden" är null<br/> eller motsvarande objekt i "värden" för en cell är null.|
| copts | [CalculationOptions](/cells/sv/python-net/aspose.cells/calculationoptions) | Alternativen för att beräkna formel.<br/> Vanligtvis bör egenskapen [CalculationOptions.recursive](/cells/sv/python-net/aspose.cells/calculationoptions#recursive) vara falsk av hänsyn till prestanda.|



###  Se även
* modul [aspose.cells](../../)
* klass [Cell](/cells/sv/python-net/aspose.cells/cell)
