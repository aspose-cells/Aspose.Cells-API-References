---
title: add metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 20
url: /sv/python-net/aspose.cells/formatconditioncollection/add/
is_root: false
---
##  add(cell_area, type, operator_type, formula1, formula2) {#CellArea-FormatConditionType-OperatorType-str-str}
Lägger till ett formateringsvillkor och påverkad cellring till FormatConditions
Formatvillkoren kan innehålla upp till tre villkorliga format.
Referenser till de andra arken är inte tillåtna i formlerna för villkorlig formatering.


###  Returnerar

[0]:Formatera villkorsobjektindex;[1] Påverkat cellrangindex.


```python
def add(self, cell_area, type, operator_type, formula1, formula2):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| cell_area | [CellArea](/cells/sv/python-net/aspose.cells/cellarea) | Villkorligt formaterat cellområde.|
| type | [FormatConditionType](/cells/sv/python-net/aspose.cells/formatconditiontype) | Typ av villkorlig formatering. Det kan vara en av medlemmarna i FormatConditionType.|
| operator_type | [OperatorType](/cells/sv/python-net/aspose.cells/operatortype) | Jämförelseoperatör. Det kan vara en av medlemmarna i OperatorType.|
| formula1 | str | Värdet eller uttrycket som är kopplat till villkorlig formatering.|
| formula2 | str | Värdet eller uttrycket som är kopplat till villkorlig formatering|



###  Se även
* modul [aspose.cells](../../)
* klass [FormatConditionCollection](/cells/sv/python-net/aspose.cells/formatconditioncollection)
