---
title: metodo get_dependents_in_calculation
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 100
url: /it/python-net/aspose.cells/cell/get_dependents_in_calculation/
is_root: false
---
##  get_dependents_in_calculation(recursive) {#bool}
Ottiene tutte le celle il cui risultato calcolato dipende da questa cella.


###  ritorna

Enumeratore per enumerare tutti i dipendenti (oggetti Cell)


```python
def get_dependents_in_calculation(self, recursive):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| recursive | bool | Se restituisce quei dipendenti che non fanno riferimento direttamente a questa cella<br/> ma riferimento ad altri fogli di questa cella|
###  Osservazioni

Per utilizzare questo metodo, assicurati che la cartella di lavoro sia stata impostata con il valore vero per
[FormulaSettings.enable_calculation_chain](/cells/it/python-net/aspose.cells/formulasettings#enable_calculation_chain) ed è stato interamente calcolato con questa impostazione.
Se non è presente alcun riferimento alla formula per questa cella, verrà restituito null.
###  Esempio

```python
from aspose.cells import Workbook

workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A1").formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2"
cells.get("A2").formula = "=IF(TRUE,B2,B1)"
workbook.settings.formula_settings.enable_calculation_chain = True
workbook.calculate_formula()
en = cells.get("B1").get_dependents_in_calculation(False)
print("B1's calculation dependents:")
for c in en:
    print(c.name)
en = cells.get("B2").get_dependents_in_calculation(False)
print("B2's calculation dependents:")
for c in en:
    print(c.name)

```



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Cell](/cells/it/python-net/aspose.cells/cell)
