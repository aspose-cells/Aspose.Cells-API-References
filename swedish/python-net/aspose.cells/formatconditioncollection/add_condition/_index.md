---
title: add_condition metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 40
url: /sv/python-net/aspose.cells/formatconditioncollection/add_condition/
is_root: false
---
##  add_condition(type) {#FormatConditionType}
Lägg till ett formatvillkor.


###  Returnerar

Formateringsvillkor objektindex;


```python
def add_condition(self, type):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| type | [FormatConditionType](/cells/sv/python-net/aspose.cells/formatconditiontype) | Formatvillkorstyp.|


##  add_condition(type, operator_type, formula1, formula2) {#FormatConditionType-OperatorType-str-str}
Lägger till ett formateringsvillkor.


###  Returnerar

Formateringsvillkor objektindex;


```python
def add_condition(self, type, operator_type, formula1, formula2):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| type | [FormatConditionType](/cells/sv/python-net/aspose.cells/formatconditiontype) | [FormatConditionType](/cells/sv/python-net/aspose.cells/formatconditiontype) för villkorlig formatering.<br/> Det kan vara en av medlemmarna i FormatConditionType.|
| operator_type | [OperatorType](/cells/sv/python-net/aspose.cells/operatortype) | Jämförelsen [OperatorType](/cells/sv/python-net/aspose.cells/operatortype).<br/> Det kan vara en av medlemmarna i OperatorType.|
| formula1 | str | Värdet eller uttrycket som är kopplat till villkorlig formatering.<br/>Om inmatningsvärdet börjar med '=' kommer det att tas som formel.<br/>Annars kommer det att tas som vanligt värde (text, nummer, bool).<br/> För textvärde som börjar med '=' kan användaren mata in det som formel i formatet: "=\"=...\"".|
| formula2 | str | Värdet eller uttrycket som är kopplat till villkorlig formatering.<br/>Inmatningsformatet är detsamma som formel1|



###  Se även
* modul [aspose.cells](../../)
* klass [FormatConditionCollection](/cells/sv/python-net/aspose.cells/formatconditioncollection)
* klass [FormatConditionType](/cells/sv/python-net/aspose.cells/formatconditiontype)
* klass [OperatorType](/cells/sv/python-net/aspose.cells/operatortype)
