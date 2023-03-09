---
title: get_list_value metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 70
url: /sv/python-net/aspose.cells/validation/get_list_value/
is_root: false
---
##  get_list_value(row, column) {#int-int}
Hämta värdet för lista för valideringen för den angivna cellen.


###  Returnerar

Värdet för att skapa listan över denna validering för den angivna cellen.
Om listan hänvisar till ett område, kommer det returnerade värdet att vara ett [ReferredArea](/cells/sv/python-net/aspose.cells/referredarea)-objekt;
Annars kan det returnerade värdet vara null, objekt[] eller enkelt objekt.


```python
def get_list_value(self, row, column):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| row | int | Radindex.|
| column | int | Kolumnindex.|
###  Anmärkningar

Endast för validering vars typ är List och har tillämpats på en given cell,
annars kommer null att returneras.


###  Se även
* modul [aspose.cells](../../)
* klass [ReferredArea](/cells/sv/python-net/aspose.cells/referredarea)
* klass [Validation](/cells/sv/python-net/aspose.cells/validation)
