---
title: get_precedents_in_calculation metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 190
url: /sv/python-net/aspose.cells/cell/get_precedents_in_calculation/
is_root: false
---
##  get_precedents_in_calculation() {#}
Hämtar alla prejudikat (referens till celler i aktuell arbetsbok) som används av denna cells formel när den beräknas.


###  Returnerar

Enumerator för att räkna upp alla referenser (ReferredArea)


```python
def get_precedents_in_calculation(self):
    ...
```


###  Anmärkningar

Denna metod kan bara fungera med situationen att [FormulaSettings.enable_calculation_chain](/cells/sv/python-net/aspose.cells/formulasettings#enable_calculation_chain)
är sant för arbetsboken och arbetsboken har beräknats helt.
Om den här cellen inte är en formel eller den inte refererar till några andra celler kommer null att returneras.
###  Exempel

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



###  Se även
* modul [aspose.cells](../../)
* klass [Cell](/cells/sv/python-net/aspose.cells/cell)
