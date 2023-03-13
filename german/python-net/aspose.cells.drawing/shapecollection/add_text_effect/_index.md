---
title: add_text_effect Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 330
url: /de/python-net/aspose.cells.drawing/shapecollection/add_text_effect/
is_root: false
---
##  add_text_effect(effect, text, font_name, size, font_bold, font_italic, upper_left_row, top, upper_left_column, left, height, width) {#MsoPresetTextEffect-str-str-int-bool-bool-int-int-int-int-int-int}
Fügt ein WordArt-Objekt ein.


###  Kehrt zurück

Gibt ein Shape-Objekt zurück, das das neue WordArt-Objekt darstellt.


```python
def add_text_effect(self, effect, text, font_name, size, font_bold, font_italic, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| effect | [MsoPresetTextEffect](/cells/de/python-net/aspose.cells.drawing/msopresettexteffect) | Der voreingestellte mso-Texteffekttyp.|
| text | str | Der WordArt-Text.|
| font_name | str | Der Schriftartname.|
| size | int | Die Schriftgröße|
| font_bold | bool | Gibt an, ob die Schriftart fett ist.|
| font_italic | bool | Gibt an, ob die Schriftart kursiv ist.|
| upper_left_row | int | Zeilenindex oben links.|
| top | int | Stellt den vertikalen Versatz der Form von der linken Zeile in Pixeleinheiten dar.|
| upper_left_column | int | Spaltenindex oben links.|
| left | int |Stellt den horizontalen Versatz der Form von der linken Spalte in Pixeleinheiten dar.|
| height | int | Stellt die Höhe der Form in Pixeleinheiten dar.|
| width | int | Stellt die Breite der Form in Pixeleinheiten dar.|

###  Beispiel

```python
from aspose.cells.drawing import MsoPresetTextEffect

# add a WordArt
wordArt1 = shapes.add_text_effect(MsoPresetTextEffect.TEXT_EFFECT10, "WordArt", "arial", 18, False, False, 3, 0, 3, 0, 200, 50)

```



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [ShapeCollection](/cells/de/python-net/aspose.cells.drawing/shapecollection)
