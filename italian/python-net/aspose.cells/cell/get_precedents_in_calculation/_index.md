---
title: metodo get_precedents_in_calculation
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 190
url: /it/python-net/aspose.cells/cell/get_precedents_in_calculation/
is_root: false
---
##  get_precedents_in_calculation() {#}
Ottiene tutti i precedenti (riferimento alle celle nella cartella di lavoro corrente) utilizzati dalla formula di questa cella durante il calcolo.


###  ritorna

Enumeratore per enumerare tutti i riferimenti (Area Riferita)


```python
def get_precedents_in_calculation(self):
    ...
```


###  Osservazioni

Questo metodo può funzionare solo con la situazione che [FormulaSettings.enable_calculation_chain](/cells/it/python-net/aspose.cells/formulasettings#enable_calculation_chain)
è vero per la cartella di lavoro e la cartella di lavoro è stata calcolata completamente.
Se questa cella non è una formula o non fa riferimento ad altre celle, verrà restituito null.
###  Esempi

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



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Cell](/cells/it/python-net/aspose.cells/cell)
