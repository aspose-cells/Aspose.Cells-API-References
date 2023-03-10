---
title: calculate_formula Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 80
url: /de/python-net/aspose.cells/worksheet/calculate_formula/
is_root: false
---
##  calculate_formula(formula) {#str}
Berechnet eine Formel.


###  Kehrt zurück

Berechnetes Formelergebnis.


```python
def calculate_formula(self, formula):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| formula | str | Zu berechnende Formel.|


##  calculate_formula(formula, opts) {#str-CalculationOptions}
Berechnet eine Formel.


###  Kehrt zurück

Berechnetes Formelergebnis.


```python
def calculate_formula(self, formula, opts):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| formula | str | Zu berechnende Formel.|
| opts | [CalculationOptions](/cells/de/python-net/aspose.cells/calculationoptions) | Optionen zur Berechnung der Formel|


##  calculate_formula(options, recursive) {#CalculationOptions-bool}
Berechnet alle Formeln in diesem Arbeitsblatt.



```python
def calculate_formula(self, options, recursive):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| options | [CalculationOptions](/cells/de/python-net/aspose.cells/calculationoptions) | Berechnungsmöglichkeiten|
| recursive | bool | True bedeutet, wenn die Zellen des Arbeitsblatts von den Zellen anderer Arbeitsblätter abhängen,<br/>die abhängigen Zellen in anderen Arbeitsblättern werden ebenfalls berechnet.<br/> Falsch bedeutet, dass alle Formeln im Arbeitsblatt berechnet wurden und die Werte richtig sind.|


##  calculate_formula(recursive, ignore_error, custom_function) {#bool-bool-ICustomFunction}
Berechnet alle Formeln in diesem Arbeitsblatt.



```python
def calculate_formula(self, recursive, ignore_error, custom_function):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| recursive | bool | True bedeutet, wenn die Zellen des Arbeitsblatts von den Zellen anderer Arbeitsblätter abhängen,<br/>die abhängigen Zellen in anderen Arbeitsblättern werden ebenfalls berechnet.<br/> Falsch bedeutet, dass alle Formeln im Arbeitsblatt berechnet wurden und die Werte richtig sind.|
| ignore_error | bool | Gibt an, ob der Fehler beim Berechnen von Formeln ausgeblendet wird.<br/> Der Fehler kann eine nicht unterstützte Funktion, externe Links usw. sein.|
| custom_function | [ICustomFunction](/cells/de/python-net/aspose.cells/icustomfunction) | Die Berechnungsfunktionen für benutzerdefinierte Formeln erweitern die Berechnungs-Engine.|
###  Bemerkungen

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen,
Bitte verwenden Sie die Methode CalculateFormula (CalculationOptions, bool).
 Diese Methode wird 12 Monate später seit August 2020 entfernt.
Aspose entschuldigt sich für etwaige Unannehmlichkeiten.


###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Worksheet](/cells/de/python-net/aspose.cells/worksheet)
