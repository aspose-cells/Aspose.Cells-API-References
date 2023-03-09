---
title: calculate_formula metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 40
url: /sv/python-net/aspose.cells/workbook/calculate_formula/
is_root: false
---
##  calculate_formula() {#}
Beräknar resultatet av formler.



```python
def calculate_formula(self):
    ...
```


###  Anmärkningar

För alla formler som stöds, se listan på https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions

##  calculate_formula(ignore_error) {#bool}

Beräknar resultatet av formler.



```python
def calculate_formula(self, ignore_error):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| ignore_error | bool | Indikerar om dölj felet i beräkningsformler. Felet kan vara en funktion som inte stöds, externa länkar, etc.|


##  calculate_formula(options) {#CalculationOptions}
Beräkna formler i denna arbetsbok.



```python
def calculate_formula(self, options):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| options | [CalculationOptions](/cells/sv/python-net/aspose.cells/calculationoptions) | Alternativ för beräkning|


##  calculate_formula(ignore_error, custom_function) {#bool-ICustomFunction}
Beräknar resultatet av formler.



```python
def calculate_formula(self, ignore_error, custom_function):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| ignore_error | bool | Indikerar om dölj felet i beräkningsformler. Felet kan vara en funktion som inte stöds, externa länkar, etc.|
| custom_function | [ICustomFunction](/cells/sv/python-net/aspose.cells/icustomfunction) | Den anpassade formelberäkningen fungerar för att utöka beräkningsmotorn.|
###  Anmärkningar

OBS: Denna medlem är nu föråldrad. Istället,
använd metoden CalculateFormula(CalculationOptions).
 Denna metod kommer att tas bort 12 månader senare sedan augusti 2020.
Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.


###  Se även
* modul [aspose.cells](../../)
* klass [Workbook](/cells/sv/python-net/aspose.cells/workbook)
