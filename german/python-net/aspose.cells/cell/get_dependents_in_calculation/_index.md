---
title: get_dependents_in_calculation Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 100
url: /de/python-net/aspose.cells/cell/get_dependents_in_calculation/
is_root: false
---
##  get_dependents_in_calculation(recursive) {#bool}
Ruft alle Zellen ab, deren berechnetes Ergebnis von dieser Zelle abhängt.


###  Kehrt zurück

Enumerator zum Aufzählen aller abhängigen Objekte (Cell-Objekte)


```python
def get_dependents_in_calculation(self, recursive):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| recursive | bool | Ob gibt die abhängigen Elemente zurück, die nicht direkt auf diese Zelle verweisen<br/> aber Verweis auf andere Blätter dieser Zelle|
###  Bemerkungen

Um diese Methode zu verwenden, stellen Sie bitte sicher, dass die Arbeitsmappe mit dem wahren Wert für festgelegt wurde
[FormulaSettings.enable_calculation_chain](/cells/de/python-net/aspose.cells/formulasettings#enable_calculation_chain) und wurde mit dieser Einstellung vollständig berechnet.
Wenn es keinen Formelbezug zu dieser Zelle gibt, wird null zurückgegeben.
###  Beispiel

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



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Cell](/cells/de/python-net/aspose.cells/cell)
