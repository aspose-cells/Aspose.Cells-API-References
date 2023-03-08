---
title: get_list_value Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 70
url: /de/python-net/aspose.cells/validation/get_list_value/
is_root: false
---
##  get_list_value(row, column) {#int-int}
Rufen Sie den Wert für die Liste der Validierung für die angegebene Zelle ab.


###  Kehrt zurück

Der Wert zum Erstellen der Liste dieser Validierung für die angegebene Zelle.
Wenn die Liste auf einen Bereich verweist, ist der zurückgegebene Wert ein [ReferredArea](/cells/de/python-net/aspose.cells/referredarea)-Objekt;
Andernfalls kann der zurückgegebene Wert null, object[] oder einfaches Objekt sein.


```python
def get_list_value(self, row, column):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| row | int | Der Zeilenindex.|
| column | int | Der Spaltenindex.|
###  Bemerkungen

Nur für die Validierung, deren Typ Liste ist und auf eine bestimmte Zelle angewendet wurde,
andernfalls wird null zurückgegeben.


###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [ReferredArea](/cells/de/python-net/aspose.cells/referredarea)
* Klasse [Validation](/cells/de/python-net/aspose.cells/validation)
