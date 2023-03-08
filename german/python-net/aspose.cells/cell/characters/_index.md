---
title: characters Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 30
url: /de/python-net/aspose.cells/cell/characters/
is_root: false
---
##  characters(start_index, length) {#int-int}
Gibt ein Characters-Objekt zurück, das einen Bereich von characters im Zellentext darstellt.


###  Kehrt zurück

Zeichenobjekt.


```python
def characters(self, start_index, length):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| start_index | int | Der Index des Zeichenanfangs.|
| length | int | Die Anzahl der Zeichen.|
###  Bemerkungen

Diese Methode funktioniert nur bei Zellen mit Zeichenfolgenwerten.
###  Beispiel


```python
from aspose.cells import Workbook
from aspose.pydrawing import Color

excel = Workbook()
cells = excel.worksheets[0].cells
cells.get("A1").put_value("Helloworld")
cells.get("A1").characters(5, 5).font.is_bold = True
cells.get("A1").characters(5, 5).font.color = Color.blue

```



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Cell](/cells/de/python-net/aspose.cells/cell)
