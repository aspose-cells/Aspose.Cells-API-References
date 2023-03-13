---
title: get_dependents_in_calculation Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 390
url: /de/python-net/aspose.cells/cells/get_dependents_in_calculation/
is_root: false
---
##  get_dependents_in_calculation(row, column, recursive) {#int-int-bool}
Ruft alle Zellen ab, deren berechnetes Ergebnis von einer bestimmten Zelle abhängt.


###  Kehrt zurück

Enumerator zum Aufzählen aller abhängigen Objekte (Cell-Objekte)


```python
def get_dependents_in_calculation(self, row, column, recursive):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| row | int | Zeilenindex der spezifischen Zelle|
| column | int | Spaltenindex der spezifischen Zelle.|
| recursive | bool | Ob gibt die abhängigen Elemente zurück, die nicht direkt auf die bestimmte Zelle verweisen<br/> aber Verweis auf andere Blätter dieser Zelle.|
###  Bemerkungen

Um diese Methode zu verwenden, stellen Sie bitte sicher, dass die Arbeitsmappe mit dem wahren Wert für festgelegt wurde
[FormulaSettings.enable_calculation_chain](/cells/de/python-net/aspose.cells/formulasettings#enable_calculation_chain) und wurde mit dieser Einstellung vollständig berechnet.
Wenn es keinen Formelbezug zu dieser Zelle gibt, wird null zurückgegeben.
Weitere Details und Beispiele finden Sie unter [Cell.get_dependents_in_calculation(recursive)](/cells/de/python-net/aspose.cells/cell/get_dependents_in_calculation)


###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Cells](/cells/de/python-net/aspose.cells/cells)
