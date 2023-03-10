---
title: get_dependents_in_calculation metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 390
url: /sv/python-net/aspose.cells/cells/get_dependents_in_calculation/
is_root: false
---
##  get_dependents_in_calculation(row, column, recursive) {#int-int-bool}
Hämtar alla celler vars beräknade resultat beror på specifik cell.


###  Returnerar

Enumerator för att räkna upp alla anhöriga (Cell objekt)


```python
def get_dependents_in_calculation(self, row, column, recursive):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| row | int | Radindex för den specifika cellen|
| column | int | Kolumnindex för den specifika cellen.|
| recursive | bool | Om returnerar de beroende som inte refererar till den specifika cellen direkt<br/> men hänvisning till andra blad i den cellen.|
###  Anmärkningar

För att använda den här metoden, se till att arbetsboken har ställts in med sant värde för
[FormulaSettings.enable_calculation_chain](/cells/sv/python-net/aspose.cells/formulasettings#enable_calculation_chain) och har beräknats helt med denna inställning.
Om det inte finns någon formelreferens till den här cellen kommer null att returneras.
För mer information och exempel, se [Cell.get_dependents_in_calculation(recursive)](/cells/sv/python-net/aspose.cells/cell/get_dependents_in_calculation)


###  Se även
* modul [aspose.cells](../../)
* klass [Cells](/cells/sv/python-net/aspose.cells/cells)
