---
title: get_style_in_pool Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 190
url: /de/python-net/aspose.cells/workbook/get_style_in_pool/
is_root: false
---
##  get_style_in_pool(index) {#int}
Holt den Stil in den Stilpool.
Alle Stile in der Arbeitsmappe werden in einem Pool gesammelt.
Es gibt nur einen einfachen Referenzindex in den Zellen.


###  Kehrt zurück

Der Stil im Pool entspricht dem angegebenen Index, kann null sein.


```python
def get_style_in_pool(self, index):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| index | int | Der Index.|
###  Bemerkungen

Wenn der zurückgegebene Stil geändert wird, wird der Stil aller Zellen (die sich auf diesen Stil beziehen) geändert.


###  Siehe auch

* Modul [aspose.cells](../../)
* Klasse [Workbook](/cells/de/python-net/aspose.cells/workbook)
