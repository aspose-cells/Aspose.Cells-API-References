---
title: add_condition Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 40
url: /de/python-net/aspose.cells/formatconditioncollection/add_condition/
is_root: false
---
##  add_condition(type) {#FormatConditionType}
Fügen Sie eine Formatbedingung hinzu.


###  Kehrt zurück

Bedingungsobjektindex formatieren;


```python
def add_condition(self, type):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| type | [FormatConditionType](/cells/de/python-net/aspose.cells/formatconditiontype) | Bedingungstyp formatieren.|


##  add_condition(type, operator_type, formula1, formula2) {#FormatConditionType-OperatorType-str-str}
Fügt eine Formatierungsbedingung hinzu.


###  Kehrt zurück

Bedingungsobjektindex formatieren;


```python
def add_condition(self, type, operator_type, formula1, formula2):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| type | [FormatConditionType](/cells/de/python-net/aspose.cells/formatconditiontype) | [FormatConditionType](/cells/de/python-net/aspose.cells/formatconditiontype) der bedingten Formatierung.<br/> Es könnte eines der Mitglieder von FormatConditionType sein.|
| operator_type | [OperatorType](/cells/de/python-net/aspose.cells/operatortype) | Der Vergleich [OperatorType](/cells/de/python-net/aspose.cells/operatortype).<br/> Es könnte eines der Mitglieder von OperatorType sein.|
| formula1 | str | Der Wert oder Ausdruck, der der bedingten Formatierung zugeordnet ist.<br/>Wenn der Eingabewert mit '=' beginnt, wird er als Formel angenommen.<br/>Andernfalls wird es als einfacher Wert (Text, Zahl, Bool) genommen.<br/> Für einen Textwert, der mit '=' beginnt, kann der Benutzer ihn als Formel im Format "=\"=...\"" eingeben.|
| formula2 | str | Der Wert oder Ausdruck, der der bedingten Formatierung zugeordnet ist.<br/>Das Eingabeformat ist dasselbe wie bei formula1|



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [FormatConditionCollection](/cells/de/python-net/aspose.cells/formatconditioncollection)
* Klasse [FormatConditionType](/cells/de/python-net/aspose.cells/formatconditiontype)
* Klasse [OperatorType](/cells/de/python-net/aspose.cells/operatortype)
