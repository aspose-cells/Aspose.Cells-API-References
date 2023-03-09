---
title: get_precedents_in_calculation método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 190
url: /es/python-net/aspose.cells/cell/get_precedents_in_calculation/
is_root: false
---
##  get_precedents_in_calculation() {#}
Obtiene todos los precedentes (referencia a celdas en el libro de trabajo actual) usados por la fórmula de esta celda mientras se calcula.


###  Devoluciones

Enumerador para enumerar todas las referencias (ReferredArea)


```python
def get_precedents_in_calculation(self):
    ...
```


###  Observaciones

Este método solo puede funcionar con la situación de que [FormulaSettings.enable_calculation_chain](/cells/es/python-net/aspose.cells/formulasettings#enable_calculation_chain)
es cierto para el libro de trabajo y el libro de trabajo se ha calculado completamente.
Si esta celda no es una fórmula o no hace referencia a ninguna otra celda, se devolverá un valor nulo.
###  Ejemplo

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



###  Ver también
* módulo [aspose.cells](../../)
* clase [Cell](/cells/es/python-net/aspose.cells/cell)
