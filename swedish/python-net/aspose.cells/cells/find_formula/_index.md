---
title: find_formula metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 300
url: /sv/python-net/aspose.cells/cells/find_formula/
is_root: false
---
##  find_formula(formula, previous_cell) {#str-Cell}
Hittar cellen med inmatningssträngen.


###  Returnerar

Cell objekt.


```python
def find_formula(self, formula, previous_cell):
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
 och LookAtType som LookAtType.EntireContent.
 Denna medlem kommer att tas bort 12 månader senare sedan november 2018.
Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.


###  Se även
* modul [aspose.cells](../../)
* klass [Cells](/cells/sv/python-net/aspose.cells/cells)
