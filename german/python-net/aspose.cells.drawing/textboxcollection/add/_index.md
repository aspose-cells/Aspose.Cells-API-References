---
title: add Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 20
url: /de/python-net/aspose.cells.drawing/textboxcollection/add/
is_root: false
---
##  add(upper_left_row, upper_left_column, height, width) {#int-int-int-int}
Fügt der Sammlung ein Textfeld hinzu.


###  Kehrt zurück

[TextBox](/cells/de/python-net/aspose.cells.drawing/textbox) Objektindex.


```python
def add(self, upper_left_row, upper_left_column, height, width):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| upper_left_row | int | Zeilenindex oben links.|
| upper_left_column | int | Spaltenindex oben links.|
| height | int | Höhe des Textfelds in Pixeleinheiten.|
| width | int | Breite des Textfelds in Pixeleinheiten.|

###  Beispiel

```python

# add a TextBox
index2 = textBoxCollection.add(1, 1, 50, 100)

```



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [TextBox](/cells/de/python-net/aspose.cells.drawing/textbox)
* Klasse [TextBoxCollection](/cells/de/python-net/aspose.cells.drawing/textboxcollection)
