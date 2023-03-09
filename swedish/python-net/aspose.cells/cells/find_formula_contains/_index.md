---
title: find_formula_contains metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 310
url: /sv/python-net/aspose.cells/cells/find_formula_contains/
is_root: false
---
##  find_formula_contains(formula, previous_cell) {#str-Cell}
Hittar cellen med formeln som innehåller inmatningssträngen.


###  Returnerar

Cell objekt.


```python
def find_formula_contains(self, formula, previous_cell):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| formula | str | Formeln att söka efter.|
| previous_cell | [Cell](/cells/sv/python-net/aspose.cells/cell) | Föregående cell med samma formel. Denna parameter kan ställas in på null om du söker från början.|
###  Anmärkningar

Returnerar null (ingenting) om ingen cell hittas.
OBS: Denna medlem är nu föråldrad. Istället,
använd metoden Cells.Find(object,Cell,FindOptions) med LookInType som LookInType.OnlyFormulas
 och LookAtType som LookAtType.Contains.
 Denna medlem kommer att tas bort 12 månader senare sedan november 2018.
Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.


###  Se även
* modul [aspose.cells](../../)
* klass [Cells](/cells/sv/python-net/aspose.cells/cells)
