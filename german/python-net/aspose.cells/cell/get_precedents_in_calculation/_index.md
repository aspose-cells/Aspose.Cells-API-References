---
title: get_precedents_in_calculation Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 190
url: /de/python-net/aspose.cells/cell/get_precedents_in_calculation/
is_root: false
---
##  get_precedents_in_calculation() {#}
Ruft alle Präzedenzfälle (Verweis auf Zellen in der aktuellen Arbeitsmappe) ab, die von der Formel dieser Zelle während der Berechnung verwendet werden.


###  Kehrt zurück

Enumerator zum Aufzählen aller Referenzen (ReferredArea)


```python
def get_precedents_in_calculation(self):
    ...
```


###  Bemerkungen

Diese Methode kann nur mit der Situation funktionieren, dass [FormulaSettings.enable_calculation_chain](/cells/de/python-net/aspose.cells/formulasettings#enable_calculation_chain)
für die Arbeitsmappe wahr ist und die Arbeitsmappe vollständig berechnet wurde.
Wenn diese Zelle keine Formel ist oder auf keine andere Zelle verweist, wird null zurückgegeben.
###  Beispiel

```python
from aspose.cells import Workbook

workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A2").formula = "=IF(TRUE,B2,B1)"
workbook.settings.formula_settings.enable_calculation_chain = True
workbook.calculate_formula()
en = cells.get("A2").get_precedents_in_calculation()
print("A2's calculation precedents:")
for r in en:
    print(r)

```



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Cell](/cells/de/python-net/aspose.cells/cell)
