---
title: calculate_formula Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 40
url: /de/python-net/aspose.cells/workbook/calculate_formula/
is_root: false
---
##  calculate_formula() {#}
Berechnet das Ergebnis von Formeln.



```python
def calculate_formula(self):
    ...
```


###  Bemerkungen

Alle unterstützten Formeln finden Sie in der Liste unter https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions

##  calculate_formula(ignore_error) {#bool}

Berechnet das Ergebnis von Formeln.



```python
def calculate_formula(self, ignore_error):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| ignore_error | bool | Gibt an, ob der Fehler beim Berechnen von Formeln ausgeblendet wird. Der Fehler kann eine nicht unterstützte Funktion, externe Links usw. sein.|


##  calculate_formula(options) {#CalculationOptions}
Berechnungsformeln in diesem Arbeitsbuch.



```python
def calculate_formula(self, options):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| options | [CalculationOptions](/cells/de/python-net/aspose.cells/calculationoptions) | Berechnungsmöglichkeiten|


##  calculate_formula(ignore_error, custom_function) {#bool-ICustomFunction}
Berechnet das Ergebnis von Formeln.



```python
def calculate_formula(self, ignore_error, custom_function):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| ignore_error | bool | Gibt an, ob der Fehler beim Berechnen von Formeln ausgeblendet wird. Der Fehler kann eine nicht unterstützte Funktion, externe Links usw. sein.|
| custom_function | [ICustomFunction](/cells/de/python-net/aspose.cells/icustomfunction) | Die Berechnungsfunktionen für benutzerdefinierte Formeln erweitern die Berechnungs-Engine.|
###  Bemerkungen

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen,
Bitte verwenden Sie die Methode CalculateFormula (CalculationOptions).
 Diese Methode wird 12 Monate später seit August 2020 entfernt.
Aspose entschuldigt sich für etwaige Unannehmlichkeiten.


###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Workbook](/cells/de/python-net/aspose.cells/workbook)
