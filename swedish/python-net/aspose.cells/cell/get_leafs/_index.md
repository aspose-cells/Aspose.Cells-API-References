---
title: get_leafs metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 160
url: /sv/python-net/aspose.cells/cell/get_leafs/
is_root: false
---
##  get_leafs() {#}
Hämta alla celler som refererar till denna cell direkt och behöver uppdateras när den här cellen ändras.


###  Returnerar

Enumerator för att räkna upp alla anhöriga (Cell)


```python
def get_leafs(self):
    ...
```


###  Anmärkningar

OBS: Denna klass är nu föråldrad.
använd Cell.GetDependentsInCalculation(bool) för att få alla anhöriga i beräkningskedjan.
Den här egenskapen kommer att tas bort 12 månader senare sedan maj 2022.
Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

##  get_leafs(recursive) {#bool}
Hämta alla celler som kommer att uppdateras när denna cell ändras.


###  Returnerar

Enumerator för att räkna upp alla anhöriga (Cell)


```python
def get_leafs(self, recursive):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| recursive | bool | Om returnerar de blad som inte refererar till den här cellen direkt<br/> men hänvisning till andra blad i denna cell|
###  Anmärkningar

OBS: Denna klass är nu föråldrad.
använd Cell.GetDependentsInCalculation(bool) för att få alla anhöriga i beräkningskedjan.
Den här egenskapen kommer att tas bort 12 månader senare sedan maj 2022.
Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.


###  Se även
* modul [aspose.cells](../../)
* klass [Cell](/cells/sv/python-net/aspose.cells/cell)
